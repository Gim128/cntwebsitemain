<template>
    <section>
    <div class="mx-auto max-w-screen-2xl px-4 py-8 sm:px-6 lg:px-8">
      <div class="grid grid-cols-1 gap-4 md:grid-cols-2">
        <div class="bg-[radial-gradient(ellipse_at_left,_var(--tw-gradient-stops))] from-cyan-500 via-sky-500 to-blue-500 p-8 md:p-12 lg:px-16 lg:py-24">
          <div class="mx-auto max-w-xl text-center">
            <h2 class="text-2xl font-bold text-white md:text-3xl mt-10">
              {{ $t("msgelev") }}
            </h2>
  
            <p class="hidden text-white/90 sm:mt-4 sm:block mt-3">
              {{ $t("msgtwl") }}
            </p>
  
            <div class="mt-4 md:mt-8">
              <a
                href="https://tronscan.org/#/token20/TX8yuS4sRtbSXJVtjsmR7pSDQDrioWopKS" target="_blank"
                class="inline-block rounded border border-white bg-white px-12 py-3 text-lg font-semibold text-blue-500 transition hover:bg-transparent hover:text-white focus:outline-none focus:ring focus:ring-yellow-400"
              >
                {{ $t("msgthirt") }}
              </a>
            </div>
          </div>
        </div>
  
        <div class="grid grid-cols-2 gap-4 md:grid-cols-1 lg:grid-cols-2">
          <img
            alt="Student"
            src="https://images.pexels.com/photos/6771671/pexels-photo-6771671.jpeg?auto=compress&cs=tinysrgb&w=600"
            class="h-40 w-full object-cover sm:h-56 md:h-full"
          />
  
          <img
            alt="Student"
            src="https://images.pexels.com/photos/5831671/pexels-photo-5831671.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
            class="h-40 w-full object-cover sm:h-56 md:h-full"
          />
        </div>
      </div>
    </div>
  </section>
  



</template>

<script>
export default {
  name: "CATComponent",

  methods: {
    ethereum() {
      window.open(
        "https://tronscan.io/#/token20/TX8yuS4sRtbSXJVtjsmR7pSDQDrioWopKS"
      );
    },
  },
};
</script>

<style>
</style>