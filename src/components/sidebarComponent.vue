<template>
  <div
    class="
      wrapper
      flex
      relative
      w-full
      ease-in
      transition-all
      lg:hidden
      xl:hidden
      left-0
    "
  >
    <ul
      class="
        md:py-0
        py-3
        bg-gradient-to-r
        from-sky-400
        to-blue-500
        px-30
        w-full
        items-end
        pb-1
      "
    >
      <li class="mx-4 my-5 md:my-0">
        <a
          href="#"
          class="
            block
            text-white text-xl
            font-bold
            hover:text-blue-700
            duration-500
          "
          >Home</a
        >
      </li>

      <!-- <li class="my-6 md:my-0">
        <a
          href="#"
          class="
            block
            text-blue-900 text-xl
            font-bold
            hover:text-blue-700
            duration-500
          "
          >Home</a
        >
      </li> -->

      <!-- <button class="bg-blue-800 text-white duration-500 px-6 py-2 mx-4 hover:bg-blue-400 rounded"> -->
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
  height: 100vh;
  width: 40vw;
  z-index: 99;
}
</style>