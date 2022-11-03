<template>
  <div class="w-full max-w-xl mx-auto">
    <form class="bg-white shadow-md rounded px-8 pt-6 pb-8 mb-4">
      <div class="text-center font-semibold text-2xl">Room Allocation</div>
      <div class="grid grid-cols-2 gap-4">
        <div class="mb-4">
          <label
            class="block text-gray-700 text-sm font-bold mb-2"
            for="conference-room"
          >
            Conference Room
          </label>
          <input
            v-model="capacity"
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            id="conference-room"
            type="number"
            placeholder="Capacity"
          />
          <p class="text-red-500 text-xs italic pt-4">Error message comes here</p>
        </div>
        <div class="mb-6">
          <label
            class="block text-gray-700 text-sm font-bold mb-2"
            for="room-one"
          >
            Room One
          </label>
          <InputTags v-model="roomOne" />
          <p class="text-red-500 text-xs italic">Error message comes here</p>
        </div>
        <div class="mb-6">
          <label
            class="block text-gray-700 text-sm font-bold mb-2"
            for="number"
          >
            Room Two
          </label>
          <InputTags v-model="roomTwo" />
          <p class="text-red-500 text-xs italic">Error message comes here</p>
        </div>
        <div class="mb-6">
          <label
            class="block text-gray-700 text-sm font-bold mb-2"
            for="room-three"
          >
            Room Three
          </label>
          <InputTags v-model="roomThree" />
          <p class="text-red-500 text-xs italic">Error message comes here</p>
        </div>
        <div class="mb-6">
          <label
            class="block text-gray-700 text-sm font-bold mb-2"
            for="room-four"
          >
            Room Four
          </label>
          <InputTags v-model="roomFour" />
          <p class="text-red-500 text-xs italic">Error message comes here</p>
        </div>
        <div class="mb-6">
          <label
            class="block text-gray-700 text-sm font-bold mb-2"
            for="room-five"
          >
            Room Five
          </label>
          <InputTags v-model="roomFive" />
          <p class="text-red-500 text-xs italic">Error message comes here</p>
        </div>
        <div class="mb-6">
          <label
            class="block text-gray-700 text-sm font-bold mb-2"
            for="room-six"
          >
            Room Six
          </label>
          <InputTags v-model="roomSix" />
          <p class="text-red-500 text-xs italic">Error message comes here</p>
        </div>
      </div>

      <div class="flex items-center justify-between">
        <button
          class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline w-1/2 mx-auto"
          type="button"
        >
          Submit
        </button>
      </div>
    </form>
    <p class="text-center text-gray-500 text-xs">&copy;2022 Web3Bridge.</p>
  </div>
</template>

<script>
import InputTags from "./components/InputTags.vue";
export default {
  name: "App",
  components: {
    InputTags,
  },
  data() {
    return {
      capacity: null,
      roomOne: null,
      roomTwo: null,
      roomThree: null,
      roomFour: null,
      roomFive: null,
      roomSix: null,
      tags: ["bar", "foo"],
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  margin-top: 60px;
}
</style>
