<template>
  <footer
    class="
      flex flex-gap
      text-center
      lg:text-left
      bg-gradient-to-r
      from-blue-100
      via-blue-300
      to-blue-500
      text-gray-600
      mt-20
      justify-between
      bg-cover bg-no-repeat
    "
  >
    <div class="mr-6 mx-6 py-10 text-center md:text-left justify-between">
      <div
        class="
          flex flex-row
          basis-1/3
          flex-1
          md:flex-cols-2
          lg:flex-cols-4
          gap-8
          justify-between
        "
      >
        <!-- <div class=""> -->
        <h6
          class="
            uppercase
            font-bold
            mb-4
            flex flex-row
            basis-1/3
            items-center
            justify-between
            md:justify-between
            text-4xl
          "
        >
          <img src="../assets/cnt-gold.png" class="w-20 h-20 mr-4" alt="" />
          {{ $t("msgthtyone") }}
        </h6>

        <div class="flex flex-row basis-1/3 justify-between">
          <p class="mb-4">
            <a href="#" class="text-gray-600">{{ $t("msgthtyegt") }}</a>
          </p>
        </div>

        <!-- </div> -->

        <div class="flex flex-row basis-1/3 justify-between">
          <span>{{ $t("msgftfv") }}</span>
          <a class="text-gray-600 font-semibold ml-2" href="#">{{
            $t("msgftsx")
          }}</a>
        </div>
      </div>
      <!-- <div class="text-center justify-between p-6"> -->
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterComponent",

  methods: {
    whitePaper() {
      window.open("https://www.freepik.com/");
    },
  },

  data() {
    return {
      // icons: [
      //     'mdi-facebook',
      //     'mdi-twitter',
      //     'mdi-linkedin',
      //     'mdi-instagram',
      // ],
    };
  },
};
</script>

<style scoped>
</style>

