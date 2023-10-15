<template>
  <!-- <div class="bg-gray-900 text-gray-100 py-8 px-6 shadow md:flex justify-between items-center">
    <div class="flex items-center cursor-pointer">
        <span  class="text--green-500 text-xl mr-1">Portfolio.CNT</span>
    </div>

    <span @click="MenuOpen()" class="absolute md:hidden right-6 top-1.5 cursor-pointer text-4xl">
      <v-icon :class="[open ? 'mdi-menu' : 'mdi-format-align-left']"></v-icon>
    </span>
    
    <ul class="md:flex md:items-end md:px-0 px-10 md:pb-0 pb-10 md:static absolute bg-gray-900 md:w-auto w-full top-14 duration-700 ease-in" :class="[open ? 'left-0' : 'left-[-100%]']">
        <li class="md:mx-4 md:my-0 my-6" v-for="link in Links" :key="link">
            <a :href="link.link" class="text-xl hover:text-gold-500">{{link.name}}</a>
        </li>
        <button-component />
    </ul>
  </div> -->
    <div class="flex bg-gray-900 text-gray-100 py-8 px-6 shadow md:flex justify-between items-center">
      <div>
        <!-- <span @click="portfolio" class="text-blue-500 text-xl mr-1 cursor-pointer">Potfolio.CNT</span> -->
        <span>
          <img src="../assets/cnt-gold.png" @click="portfolio" class="cursor-pointer h-10 w-10 ml-3" alt="">
        </span>
      </div>

      <div class="flex" >
        <div>
          <span @click="MenuOpen()" class=" md:hidden right-6 top-1.5 cursor-pointer text-4xl">
            <v-icon :class="[open ? 'mdi-menu' : 'mdi-format-align-left']"></v-icon>
          </span>
        </div>
        <div>
          <ul class="md:flex md:items-end md:px-0 px-10 md:pb-0 pb-10 md:static  md:w-auto w-full top-14 duration-700 ease-in" :class="[open ? 'left-0' : 'left-[-100%]']">
            <li class="md:mx-4 md:my-0 my-6" v-for="link in Links" :key="link">
                <a :href="link.link" class="text-xl hover:text-gold-500">{{link.name}}</a>
            </li>
    
            <button-component />
    
        </ul>
        </div>
      </div>
    </div>
</template>

<script>
import { ref } from 'vue'
import buttonComponent from './buttonComponent.vue'


export default {
  components: { buttonComponent },
    name: "NavbarView",
    
    methods: {
      portfolio() {
        location.reload();
      }
    },

    setup() {
      let open = ref(true)
      let Links = [
        {name: "Home", link: "#"},
        
      ]

      function MenuOpen() {
        open.value = !open.value
      }

      return {Links, open, MenuOpen}
    },


  }


</script>

<style scoped>
  @import '../assets/tailwind.css'
</style>