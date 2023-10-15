<template>
    <div class="flex bg-gray-900 text-white py-3.5 px-6 shadow md:flex justify-between items-center">
      <div class="flex items-center cursor-pointer">
          <span class="mr-3">
              <img src="../assets/cnt-gold.png" class="mr-3 w-10 h-10" alt="">
          </span>
          <h1 class="cursor-pointer hover:border-x-sky-400 text-white text-xl font-bold">CNT</h1>
      </div>

     
  
      <ul class="md:flex md:items-center md:px-0 px-10 md:pb-0 pb-10 md:static bg-gray-900 md:w-auto w-full top-14 duration-700 ease-in" :class="[open ? 'left-0' : 'left-[-100%]']">
          <li class="md:mx-4 md:my-0 my-6"> 
             <a href="#" class="text-xl hover:text-yellow-500">Home</a> 
          </li>
          <!-- <li class="md:mx-4 md-my-0 my-6"> 
            <a href="#" class="text-xl hover:text-yellow-500">Home</a> 
          </li> -->
         
         <Button>
            <button-component />
         </Button>
          
  
      </ul>
      <span  class="absolute md:hidden right-6 top-1.5 cursor-pointer text-4xl">
        <!-- <i :class="true ? 'bi-bi-x' : 'bi-bi-list-left'"></i> -->
        <img @click="MenuOpen()" src="../assets/close.svg" class="w-5 h-5 mt-10 cursor-pointer" alt="">
      </span>
    </div>
  </template>
  
  <script>
import { ref } from 'vue';
  import buttonComponent from './buttonComponent.vue';
  
  export default {
    components: { buttonComponent },
    name: "NavbarView",

    setup(){
        let open = ref({
          value:false
        })

        function MenuOpen(){
          console.log("Something Clicked");
            this.open.value = !this.open.value
        }

        return{open, MenuOpen}
    }

  }
  </script>
  
  <style>
  
  </style>