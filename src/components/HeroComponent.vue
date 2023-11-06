<template>
  <div class="hero-section">
    <main style="margin-bottom: -132px">
      <img src="../assets/bg-img-bg.webp" alt="background image" class="bg-hero">
      <div class="relative px-6 lg:px-8">
        <div class="max-w-3xl pt-12 pb-32 mx-auto sm:pt-48 sm:pb-40">
          <div>
            <div>
              <h1
                class="mb-6 text-4xl font-bold tracking-tight text-black sm:text-center sm:text-6xl"
                style="margin-top: -28px"
              >
                {{ $t("messagethree") }}
              </h1>
              <p class="mt-6 text-lg leading-8 text-black sm:text-center">
                {{ $t("msgfour") }}
              </p>
              <div
                class="flex flex-wrap mt-12 mb-8 space-x-4 md:grid-cols-3 gap-x-16 sm:justify-center"
              >
                <div
                  class="flex w-full px-6 py-2 mb-5 space-x-6 text-lg font-semibold text-indigo-700 transition bg-white border border-indigo-900 rounded sm:w-1/2 md:w-1/3 lg:w-1/3 xl:w-1/4 hover:bg-slate-200 hover:text-indigo-300 focus:outline-none focus:ring focus:ring-yellow-400"
                >
                  <img src="../assets/android.png" alt="Image 1" class="w-10 h-10 mb-3" />
                  <a
                    href="https://oss.icanlk.com/android/CNTPAY/cntpay.apk"
                    target="_blank"
                    class="inline-block px-1 py-3 text-lg font-semibold text-indigo-700 transition hover:text-indigo-700 focus:outline-none focus:ring focus:ring-indigo-500"
                  >
                  {{ $t("msgftnn") }}
                  </a>
                </div>

                <div
                  class="flex w-full px-6 py-2 mb-5 space-x-6 text-lg font-semibold text-indigo-700 transition bg-white border border-indigo-900 rounded sm:w-1/2 md:w-1/3 lg:w-1/3 xl:w-1/4 hover:bg-slate-200 hover:text-indigo-300 focus:outline-none focus:ring focus:ring-yellow-400"
                >
                  <img src="../assets/ios.png" alt="Image 2" class="w-10 h-10 mb-3" />
                  <a
                    href="https://c2c.cntpay.net/"
                    target="_blank"
                    class="inline-block px-1 py-3 text-lg font-semibold text-indigo-700 transition hover:text-indigo-700 focus:outline-none focus:ring focus:ring-indigo-500"
                  >
                  {{ $t("msgsxt") }}
                  </a>
                </div>

                <div
                  class="flex w-full px-6 py-2 mb-5 space-x-6 text-lg font-semibold text-indigo-700 transition bg-white border border-indigo-900 rounded sm:w-1/2 md:w-1/3 lg:w-1/3 xl:w-1/4 hover:bg-slate-200 hover:text-indigo-300 focus:outline-none focus:ring focus:ring-yellow-400"
                >
                  <img src="../assets/browser.png" alt="Image 3" class="w-10 h-10 mb-3" />
                  <a
                    href="https://cntpay.ogzlbnq.com/9rizw"
                    target="_blank"
                    class="inline-block px-1 py-3 text-lg font-semibold text-indigo-700 transition border-indigo-900 rounded hover:hover:bg-slate-200 hover:text-indigo-700 focus:outline-none focus:ring focus:ring-yellow-400"
                  >
                  {{ $t("msgsxtone") }}
                  </a>
                </div>
              </div>
            </div>
            <div
              class="absolute inset-x-0 top-[calc(100%-13rem)] -z-10 transform-gpu overflow-hidden blur-3xl sm:top-[calc(100%-30rem)]"
            >
              <svg
                class="relative left-[calc(50%+3rem)] h-[21.1875rem] max-w-none -translate-x-1/2 sm:left-[calc(50%+36rem)] sm:h-[42.375rem]"
                viewBox="0 0 1155 678"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill="url(#ecb5b0c9-546c-4772-8c71-4d3f06d544bc)"
                  fill-opacity=".3"
                  d="M317.219 518.975L203.852 678 0 438.341l317.219 80.634 204.172-286.402c1.307 132.337 45.083 346.658 209.733 145.248C936.936 126.058 882.053-94.234 1031.02 41.331c119.18 108.451 130.68 295.337 121.53 375.223L855 299l21.173 362.054-558.954-142.079z"
                />
                <defs>
                  <linearGradient
                    id="ecb5b0c9-546c-4772-8c71-4d3f06d544bc"
                    x1="1155.49"
                    x2="-78.208"
                    y1=".177"
                    y2="474.645"
                    gradientUnits="userSpaceOnUse"
                  >
                    <stop stop-color="#9089FC" />
                    <stop offset="1" stop-color="#FF80B5" />
                  </linearGradient>
                </defs>
              </svg>
            </div>
          </div>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  name: "HeroComponent",

  data() {
   
  },
};
</script>

<style>
  .bg-hero{
    opacity: 0.3;
    position: absolute;
    background-repeat: repeat-x !important;
    width: 100vw;
    align-items: center;
  }
</style>
