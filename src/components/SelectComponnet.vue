<template>
  <div class="isolate bg-slate-50">
    <h2
      class="mt-20 text-lg font-semibold leading-8 text-center text-indigo-700"
    >
      {{ $t("msgfort") }}
    </h2>
    <h5
      class="pb-1 mb-6 text-2xl font-bold tracking-tight text-center sm:text-center sm:text-5xl"
    >
      {{ $t("msgfiv") }}
    </h5>
    <h1 class="pb-8 mt-3 text-xl text-center">{{ $t("msgsixth") }}</h1>

    <div
      class="grid mt-12 text-center sm:grid-cols-1 md:grid-cols-2 lg:grid-cols-3"
    >
      <div @click="enableOne">
        <p
          class="
            cursor-pointer
            inline-block
            rounded-lg
            bg-white
            border-indigo-900
            px-4
            py-1.5
            text-base
            font-semibold
            leading-7
            text-indigo-700
            shadow-sm
            ring-1 ring-indigo-400
            hover:bg-slate-200 hover:ring-indigo-700
          "
        >
          {{ $t("msgsevnth") }}
          <!-- <span class="text-indigo-200" aria-hidden="true">&rarr;</span> -->
        </p>

        <p
          class="mt-3 ml-3 font-normal tracking-tight text-center cursor-pointer "
        >
          {{ $t("msgninth") }}
        </p>
      </div>
      <div @click="enableTwo">
        <p
          class="
            cursor-pointer
            inline-block
            rounded-lg
            bg-white
            border-indigo-900
            px-4
            py-1.5
            text-base
            font-semibold
            leading-7
            text-indigo-700
            shadow-sm
            ring-1 ring-indigo-400
            hover:bg-slate-200 hover:ring-indigo-700
          "
        >
          {{ $t("msgeighth") }}
          <!-- <span class="text-indigo-200" aria-hidden="true">&rarr;</span> -->
        </p>

        <p
          class="mt-3 ml-3 font-normal tracking-tight text-center cursor-pointer "
        >
          {{ $t("msgtty") }}
        </p>
      </div>
      <div @click="enableThree">
        <p
          class="
            cursor-pointer
            inline-block
            rounded-lg
            bg-white
            border-indigo-900
            px-4
            py-1.5
            text-base
            font-semibold
            leading-7
            text-indigo-700
            shadow-sm
            ring-1 ring-indigo-400
            hover:bg-slate-200 hover:ring-indigo-700
          "
        >
          {{ $t("msgtwty") }}
          <!-- <span class="text-indigo-200" aria-hidden="true">&rarr;</span> -->
        </p>

        <p
          class="mt-3 ml-3 font-normal tracking-tight text-center cursor-pointer "
        >
          {{ $t("msgtwtone") }}
        </p>
      </div>
    </div>
    <div>
      <section
        v-if="isActiveOne"
        class="grid grid-cols-4 mt-8 ml-6 mr-4 rounded"
      >
        <img
          style="padding: 20px 20px 20px 20px; border-radius: 0.75rem"
          v-for="(image, index) in webApps"
          :key="index"
          :src="image.image"
          alt=""
          height="500"
        />
      </section>

      <section
        v-if="isActiveTwo"
        class="grid grid-cols-4 mt-8 ml-6 mr-4 rounded"
      >
        <img
          style="padding: 20px 20px 20px 20px; border-radius: 0.75rem"
          v-for="(image, index) in cryptoApps"
          :key="index"
          :src="image.image"
          alt=""
          height="500"
        />
      </section>

      <section
        v-if="isActiveThree"
        class="grid grid-cols-4 mt-8 ml-6 mr-4 rounded"
      >
        <img
          style="padding: 20px 20px 20px 20px; border-radius: 0.75rem"
          v-for="(image, index) in coinApps"
          :key="index"
          :src="image.image"
          alt=""
          height="500"
        />
      </section>
    </div>
  </div>
</template>

<script>
export default {
  name: "SelectComponent",
  data() {
    return {
      isActiveOne: false,
      isActiveTwo: true,
      isActiveThree: false,

      webApps: [
        {
          title: "Web App 1",
          image:
            "https://www.analyticsinsight.net/wp-content/uploads/2022/06/Crypto-Exchanges-in-the-USA.jpg",
        },
        {
          title: "Web App 1",
          image:
            "https://www.techrepublic.com/wp-content/uploads/2022/05/best-cryptocurrency-exchanges-770x433.jpeg",
        },
        {
          title: "Web App 1",
          image:
            "https://arateg.com/static/images/Crypto-Cases_1920.jpg",
        },
        {
          title: "Web App 1",
          image:
            "https://images.livemint.com/img/2021/11/12/1600x900/CDX_1636721722418_1636721729590.jpg",
        },
        // {title: 'Web App 1', image:'https://img.freepik.com/free-photo/rows-stacks-cryptocurrency-coins-wooden-table_211682-66.jpg?w=1380&t=st=1671706102~exp=1671706702~hmac=2fb657acde425fc99a2c9d879a122569aede6645427a3c085dda7e643e14f652'},
        // {title: 'Web App 1', image:'https://img.freepik.com/free-photo/beautiful-cryptocurrency-hologram-design_23-2149250206.jpg?w=1380&t=st=1671706163~exp=1671706763~hmac=b0119c9b1c9ea2bab93a0badfd2352105d860ebaecc1bd0261b5c8d4d2b4bc52'},
       
      ],

      cryptoApps: [
        {
          title: "crypto1",
          image:
            "https://www.forbes.com/advisor/wp-content/uploads/2022/10/best_crypto_wallets.jpg",
        },
        {
          title: "crypto1",
          image:
            "https://prod.wordpress.usemultiplier.cloud/wp-content/uploads/2023/03/62398ad198b195119954dee1-1920-x-1082-p-1600.webp",
        },
        {
          title: "crypto1",
          image:
            "https://images.assettype.com/fortuneindia%2F2022-02%2Fd0057f5d-302b-4789-b2c1-033f9a69e8b7%2FCrypto_1235570383_copy.jpg?rect=0,86,2047,1151&w=1250&q=60",
        },
        {
          title: "crypto1",
          image:
            "https://media.philstar.com/photos/2022/09/26/pdax-lead_2022-09-26_13-36-19.jpg",
        },
        // {title: 'crypto1', image:'https://img.freepik.com/free-photo/flat-lay-business-concept_53876-24738.jpg?w=1380&t=st=1671706546~exp=1671707146~hmac=8e5c2df618feb767e9df93dc4249a3fd7886349e66c17e2c35c4c5eb6cbbd3e8'},
        // {title: 'crypto1', image:'https://img.freepik.com/free-photo/group-people-working-website-template_53876-25068.jpg?w=1380&t=st=1671706563~exp=1671707163~hmac=ea45529b1c6b9cfd21793d196627c1aa8957440974b968a0400385edd45cc329'},
        // {title: 'crypto1', image:'https://img.freepik.com/free-photo/hands-holding-smartphone-close-up_23-2149168656.jpg?w=1380&t=st=1671706579~exp=1671707179~hmac=9a5ac987c0b025f5083cc22ec706e687ff65823c8f4581cd78b349d81093e4aa'},
        // {title: 'crypto1', image:'https://img.freepik.com/free-photo/close-up-hand-holding-smartphone_23-2149153407.jpg?w=1380&t=st=1671773327~exp=1671773927~hmac=b81d1944d3d298501223d6c3035076914c1b2e3915c22444e251fe70f11d76eb'},
      ],

      coinApps: [
        {
          title: "coin03",
          image:
            "https://techstory.in/wp-content/uploads/2022/03/top-10-cryptocurrencies-to-Invest-2022--768x512.jpg",
        },
        {
          title: "coin03",
          image:
            "https://images.moneycontrol.com/static-mcnews/2022/03/shutterstock_1446648077.jpg?impolicy=website&width=1600&height=900",
        },
        {
          title: "coin03",
          image:
            "https://img.freepik.com/premium-photo/bitcoin-cryptocurrency-investing-concept-3d-rendering_350912-16.jpg",
        },
        {title: 'coin03', image:'https://www.cyberlink.com/prog/faceme/html/507/p/enu/img/banner_cryptocurrency.jpg'},
        // {title: 'coin03', image:'https://img.freepik.com/free-photo/ai-technology-microchip-background-digital-transformation-concept_53876-124669.jpg?w=1380&t=st=1671773092~exp=1671773692~hmac=dc7a14215cc167a923d1fee791e668ed1ab0104c6e75ac204ff952bb9f12148c'},
        // {title: 'coin03', image:'https://img.freepik.com/free-photo/man-wearing-smart-glasses-touching-virtual-screen-futuristic-technology-digital-remix_53876-104247.jpg?w=1380&t=st=1671773141~exp=1671773741~hmac=9f69f61292aec470c17401484cce8e88ea2bca58a0721fbcb5732133aaf2c8c2'},
        // {title: 'coin03', image:'https://img.freepik.com/free-photo/hologram-projector-screen-with-cloud-system-technology_53876-108502.jpg?w=1380&t=st=1671773186~exp=1671773786~hmac=0749fc624fe9582cc480dd27b96a8b6555b5bc7221c76145283c40904ce8d600'},
        // {title: 'coin03', image:'https://img.freepik.com/free-photo/rendering-abstract-futuristic-background-with-glowing-neon-blue-orange-lights_181624-19807.jpg?w=1380&t=st=1671773206~exp=1671773806~hmac=70c44b9fe48a45f4a8b51fb5284bf3491733bf63af5d691c1652f684ec2136d8'},
      ],
    };
  },

  methods: {
    enableOne() {
      this.isActiveOne = true;
      this.isActiveTwo = false;
      this.isActiveThree = false;
    },

    enableTwo() {
      this.isActiveOne = false;
      this.isActiveTwo = true;
      this.isActiveThree = false;
    },

    enableThree() {
      this.isActiveOne = false;
      this.isActiveTwo = false;
      this.isActiveThree = true;
    },
  },
};
</script>

<style>
</style>