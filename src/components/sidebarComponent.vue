<template>
  <div
    class="relative left-0 flex w-full transition-all ease-in wrapper lg:hidden xl:hidden"
  >
    <ul
      class="items-end w-full py-3 pb-1 md:py-0 bg-gradient-to-r from-sky-400 to-blue-500 px-30"
    >
      <li class="mx-4 my-5 md:my-0">
        <a
          href="#"
          class="block text-xl font-bold text-white duration-500 hover:text-blue-700"
          >Home</a
        >
      </li>

      <!-- <li class="my-6 md:my-0">
        <a
          href="#"
          class="block text-xl font-bold text-blue-900 duration-500 hover:text-blue-700"
          >Home</a
        >
      </li> -->

      <!-- <button class="px-6 py-2 mx-4 text-white duration-500 bg-blue-800 rounded hover:bg-blue-400"> -->
      <li class="my-6 md:my-0">
        <buttonComponent />
      </li>
      <!-- </button> -->
    </ul>
  </div>
</template>
<script>
import buttonComponent from "./buttonComponent.vue";

export default {
  components: {
    buttonComponent,
  },
};
</script>

<style scoped>
.wrapper ul {
  position: absolute;
  height: 32vh;
  width: 40vw;
  z-index: 99;
}
</style>