<template>
  <div class="pb-2 border border-white rounded-lg w-full">
    <input
       class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
      v-model.trim="tag"
      @keydown.enter="addTag"
      @keydown.prevent.tab="addTag"
      placeholder="Enter Developer's Tag"
    />
    <div>
      <ul class="flex items-center flex-wrap mt-2">
        <li
          class="bg-white border-solid border-[1px] border-blue-500 px-3 py-1.5 mr-1 rounded-md"
          v-for="(tag, index) in tags"
          :key="index"
        >
          <span>{{ tag }}</span>
          <span class="delete cursor-pointer" @click="tags.splice(index, 1)">&times;</span>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "InputTags",
  props: {
    value: {
      type: Array,
      default: () => [],
    },
  },
  watch: {
    tags(n) {
      this.$emit("input", n);
    },
  },

  data() {
    return {
      tag: "",
      tags: this.value || [],
    };
  },

  methods: {
    addTag() {
      console.log("lol");
      if (this.tag && !this.tags.includes(this.tag)) {
        this.tags.push(this.tag);
        this.tag = "";
      }
    },
    deleteTag(tag) {
      this.tags.splice(this.tags.indexOf(tag), 1);
    },
  },
};
</script>

<style></style>
