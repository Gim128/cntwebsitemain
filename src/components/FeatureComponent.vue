<template>
  <div class="bg-white py-18 sm:py-32 lg:py-24"> 
    <div class="px-6 mx-auto max-w-7xl lg:px-8">
        <div class="sm:text-center">
            <h2 class="text-lg font-semibold leading-8 text-indigo-700">{{ $t('msgseven') }}</h2>
            <p class="mt-2 text-2xl font-bold tracking-tight text-gray-900 sm:text-4xl">{{ $t('msgeight') }}</p>
            <p class="max-w-2xl mx-auto mt-6 text-lg leading-8 text-gray-600">
                {{ $t('msgnine') }}
            </p>
        </div>

        <div class="max-w-lg mt-20 sm:mx-auto md:max-w-none">
            <div class="grid grid-cols-1 gap-y-16 md:grid-cols-2 md:gap-x-12 md:gap-y-16">
                <div class="flex flex-col gap-6 realtive sm:flex-row md:flex-col lg:flex-row">
                    <div class="flex items-center justify-center w-12 h-12 text-white bg-indigo-100 rounded-xl sm:shrink-0">
                        <img class="max-h-[30px]"  src="../assets/dollar.png">
                    </div>
                    <div class="sm:min-w-0 sm:flex-1">
                        <p class="text-lg font-semibold leading-8 text-gray-900">{{ $t("msgtwtwo") }}</p>
                        <p class="mt-2 text-base leading-7 text-gray-600">{{ $t("msgtwthree") }}</p>
                    </div>
                </div>

                <div class="flex flex-col gap-6 realtive sm:flex-row md:flex-col lg:flex-row">
                    <div class="flex items-center justify-center w-12 h-12 text-white bg-indigo-100 rounded-xl sm:shrink-0">
                        <img class="max-h-[30px]"  src="../assets/activity.png">
                    </div>
                    <div class="sm:min-w-0 sm:flex-1">
                        <p class="text-lg font-semibold leading-8 text-gray-900">{{ $t("msgtwtfr") }}</p>
                        <p class="mt-2 text-base leading-7 text-gray-600">{{ $t("msgtwtfv") }}</p>
                    </div>
                </div>

                <div class="flex flex-col gap-6 realtive sm:flex-row md:flex-col lg:flex-row">
                    <div class="flex items-center justify-center w-12 h-12 text-white bg-indigo-100 rounded-xl sm:shrink-0">
                        <img class="max-h-[30px]"  src="../assets/business.png">
                    </div>
                    <div class="sm:min-w-0 sm:flex-1">
                        <p class="text-lg font-semibold leading-8 text-gray-900">{{ $t("msgtwtsix") }}</p>
                        <p class="mt-2 text-base leading-7 text-gray-600">{{ $t("msgtwtsvn") }}</p>
                    </div>
                </div>

                <div class="flex flex-col gap-6 realtive sm:flex-row md:flex-col lg:flex-row">
                    <div class="flex items-center justify-center w-12 h-12 text-white bg-indigo-100 rounded-xl sm:shrink-0">
                        <img class="max-h-[30px]"  src="../assets/ecosystem.png">
                    </div>
                    <div class="sm:min-w-0 sm:flex-1">
                        <p class="text-lg font-semibold leading-8 text-gray-900">{{ $t("msgtwteight") }}</p>
                        <p class="mt-2 text-base leading-7 text-gray-600">{{ $t("msgtwtnin") }}</p>
                    </div>
                </div>
                
            </div>
        </div>

    </div>
  </div>
</template>

<script>

    export default {

        data() {
            return {
                // features : [
                //     {
                //         name: this.$t("msgtwtwo"),
                //         description: this.$t("msgtwthree"),
                //         icon: require("../assets/dollar.png"),
                //     },
                //     {
                //         name: this.$t("msgtwtfr"),
                //         description: this.$t("msgtwtfv"),
                //         icon: require("../assets/activity.png"),
                //     },
                //     {
                //         name: this.$t("msgtwtsix"),
                //         description: this.$t("msgtwtsvn"),
                //         icon: require("../assets/business.png"),
                //     },
                //     {
                //         name: this.$t("msgtwteight"),
                //         description: this.$t("msgtwtnin"),
                //         icon: require("../assets/ecosystem.png"),
                //     },
                // ]
            }
        }
}

</script>

<style>

</style>