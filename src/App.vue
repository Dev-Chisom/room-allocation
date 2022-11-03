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
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            id="conference-room"
            type="text"
            placeholder="Capacity"
          />
        </div>
        <div class="mb-6">
          <label
            class="block text-gray-700 text-sm font-bold mb-2"
            for="room-one"
          >
            Room One
          </label>
          <input
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            id="room-one"
            type="room-one"
            placeholder="Number of guests"
          />
          <p class="text-red-500 text-xs italic">Error message comes here</p>
        </div>
        <div class="mb-6">
          <label
            class="block text-gray-700 text-sm font-bold mb-2"
            for="room-two"
          >
            Room Two
          </label>
          <input
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            id="room-two"
            type="room-two"
            placeholder="Number of guests"
          />
          <p class="text-red-500 text-xs italic">Error message comes here</p>
        </div>
        <div class="mb-6">
          <label
            class="block text-gray-700 text-sm font-bold mb-2"
            for="room-three"
          >
            Room Three
          </label>
          <input
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            id="room-three"
            type="room-three"
            placeholder="Number of guests"
          />
          <p class="text-red-500 text-xs italic">Error message comes here</p>
        </div>
        <div class="mb-6">
          <label
            class="block text-gray-700 text-sm font-bold mb-2"
            for="room-four"
          >
            Room Four
          </label>
          <input
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            id="room-four"
            type="room-four"
            placeholder="Number of guests"
          />
          <p class="text-red-500 text-xs italic">Error message comes here</p>
        </div>
        <div class="mb-6">
          <label
            class="block text-gray-700 text-sm font-bold mb-2"
            for="room-five"
          >
            Room Five
          </label>
          <input
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            id="room-five"
            type="room-five"
            placeholder="Number of guests"
          />
          <p class="text-red-500 text-xs italic">Error message comes here</p>
        </div>
        <div class="mb-6">
          <label
            class="block text-gray-700 text-sm font-bold mb-2"
            for="room-six"
          >
            Room Six
          </label>
          <input
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            id="room-six"
            type="room-six"
            placeholder="Number of guests"
          />
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
export default {
  name: "App",
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
