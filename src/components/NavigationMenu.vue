<template>
  <nav
    class="p-5 bg-white shadow md:flex md:items-center md:justify-between"
    style="
      background-image: url('https://i.pinimg.com/originals/fa/b7/ca/fab7ca4ae20651bd1da35b1e00824669.jpg');
    "
  >
    <sidebarComponent v-if="isSidebarOpen" />
    <div class="flex justify-between items-center">
      <span>
        <img class="h-12 inline mr-3" src="../assets/cn-red-two.png" alt="" />
        <h2 class="inline text-2xl font-bold">CNT</h2>
      </span>

      <span class="text-3xl cursor-pointer mx-2 md:hidden block">
        <ion-icon name="menu" @click="toggleSidebar"></ion-icon>
      </span>
    </div>

    <ul
      class="
        md:flex md:items-center
        z-[-1]
        md:z-auto md:static
        absolute
        bg-white
        w-full
        left-0
        md:w-auto md:py-0
        py-4
        md:pb-0
        pb-10
        md:pl-0
        pl-7
        md:opacity-100
        opacity-0
        top-[-400px]
        transition-all
        duration-500
      "
    >
      <li class="mx-4 my-6 md:my-0">
        <a href="#" class="text-xl hover:text-blue-700 duration-500">Home</a>
      </li>

      <!-- <button class="bg-blue-800 text-white duration-500 px-6 py-2 mx-4 hover:bg-blue-400 rounded"> -->
      <li>
        <button-component />
      </li>
      <!-- </button> -->
    </ul>
  </nav>
</template>
  
  <script>
import buttonComponent from "./buttonComponent.vue";
import sidebarComponent from "@/components/sidebarComponent";

export default {
  components: { buttonComponent, sidebarComponent },
  name: "navbarComponent",

  data() {
    return {
      name: "",
      isSidebarOpen: false,
    };
  },

  methods: {
    toggleSidebar() {
      this.isSidebarOpen = !this.isSidebarOpen;
    },
  },

  setup() {},
};
</script>
  

<!-- true ? "classname" : "other-classname" -->

  <style>
</style>