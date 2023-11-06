<template>
  <footer aria-label="Site Footer" class="mt-5 bg-gradient-to-r from-gray-700 via-gray-900 to-black">
    <div
      class="relative px-4 py-12 mx-auto max-w-screen-2xl sm:px-6 lg:px-8 lg:pt-24">
    
      <div class="lg:flex lg:items-end lg:justify-between">
        <div>
          <div class="flex justify-center text-white lg:justify-start">
            <img src="../assets/cnt-red-one.png" class="mr-3 h-14 w-14" alt="CNT logo">
            <span class="self-center text-2xl font-bold">CNT - OFFICIAL</span>
          </div>
          
  
          <p
            class="max-w-full mx-auto mt-6 leading-relaxed text-center text-gray-50 lg:text-left"
          >
          {{ $t("msgsxtegt") }}
          </p>
        </div>
  
        <nav aria-label="Footer Nav" class="mt-12 lg:mt-0">
          <ul
            class="flex flex-wrap justify-center gap-6 md:gap-8 lg:justify-end lg:gap-12"
          >
            <li>
              <!-- <a class="transition text-gray-50 hover:text-gray-100/75" href="#">
                {{ $t("msgsxtfor") }}
              </a> -->
              <a href="#" class="rounded-md border-white border-2  px-3.5 py-2.5 text-sm font-semibold text-white shadow-lg focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-slate-50">
                {{ $t("msgsxtfor") }}
              </a>
            </li>
  
            <li>
              <a href="#" class="rounded-md border-white border-2  px-3.5 py-2.5 text-sm font-semibold text-white shadow-lg focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-slate-50">
                {{ $t("msgsxtfive") }}
              </a>
            </li>
          </ul>
        </nav>
      </div>
  
      <p class="mt-12 text-sm text-center text-gray-50 lg:text-right">
        {{ $t("msgsxtsx") }} &copy; 2022. {{ $t("msgsxtsvn") }}.
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