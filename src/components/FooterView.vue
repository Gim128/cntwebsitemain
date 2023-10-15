<template>
  <footer aria-label="Site Footer" class="bg-gradient-to-r from-gray-700 via-gray-900 to-black mt-5">
    <div
      class="relative mx-auto max-w-screen-xl px-4 py-12 sm:px-6 lg:px-8 lg:pt-24">
    
      <div class="lg:flex lg:items-end lg:justify-between">
        <div>
          <div class="flex justify-center text-white lg:justify-start">
            <img src="../assets/cnt-red-one.png" class="h-14 w-14 mr-3" alt="CNT logo">
            <span class="self-center text-2xl font-bold">CNT - OFFICIAL</span>
          </div>
          
  
          <p
            class="mx-auto mt-6 max-w-md text-center leading-relaxed text-gray-50 lg:text-left"
          >
          Combining the stability of the Yuwan with the efficiency of blockchain technology, CNT is designed to be secure, liquid and convenient
          </p>
        </div>
  
        <nav aria-label="Footer Nav" class="mt-12 lg:mt-0">
          <ul
            class="flex flex-wrap justify-center gap-6 md:gap-8 lg:justify-end lg:gap-12"
          >
            <li>
              <a class="text-gray-50 transition hover:text-gray-100/75" href="#">
                Home
              </a>
            </li>
  
            <li>
              <a class="text-gray-50 transition hover:text-gray-100/75" href="/">
                WhitePaper
              </a>
            </li>
          </ul>
        </nav>
      </div>
  
      <p class="mt-12 text-center text-sm text-gray-50 lg:text-right">
        Copyright &copy; 2022. All rights reserved.
      </p>
    </div>
  </footer>
  
</template>

<script>
export default {
  name: "FooterView",

  data() {
    return {};
  },
};
</script>

<style scoped>
</style>