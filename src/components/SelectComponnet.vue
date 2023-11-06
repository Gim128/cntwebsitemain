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
    <!-- <div>
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
    </div> -->

    <v-row class="imageRow">
      <v-col
        cols="6"
        sm="4"
      >
        <v-img
          src="../assets/01.png"
          gradient="to top right, rgba(100,115,201,.33), rgba(25,32,72,.7)"
        ></v-img>
      </v-col>
  
      <v-col
        cols="6"
        sm="4"
      >
        <v-img src="../assets/02.jpg">
          <div class="fill-height bottom-gradient"></div>
        </v-img>
      </v-col>
  
      <v-col
        cols="6"
        sm="4"
      >
        <v-img src="../assets/03.jpg">
          <div class="fill-height repeating-gradient"></div>
        </v-img>
      </v-col>
    </v-row>
    
  </div>
</template>

<script>
export default {
  name: "SelectComponent",
  data() {
    return {
      isActiveOne: true,
      isActiveTwo: false,
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
  
      ],

      coinApps: [
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

<style scoped>

  .imageRow{
    margin-top: 8px;
    margin-right: 3px;
    margin-left: 3px;
  }
  .bottom-gradient {
    background-image: linear-gradient(to top, rgba(0, 0, 0, 0.4) 0%, transparent 72px);
  }

  .repeating-gradient {
    background-image: repeating-linear-gradient(-45deg,
                        rgba(255,0,0,.25),
                        rgba(255,0,0,.25) 5px,
                        rgba(0,0,255,.25) 5px,
                        rgba(0,0,255,.25) 10px
                      );
  }
</style>

