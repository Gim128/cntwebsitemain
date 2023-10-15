<template>
  <div class="bg-white py-18 sm:py-32 lg:py-24"> 
    <div class="mx-auto max-w-7xl px-6 lg:px-8">
        <div class="sm:text-center">
            <h2 class="text-lg font-semibold leading-8 text-indigo-700">{{ $t('msgseven') }}</h2>
            <p class="mt-2 text-2xl font-bold tracking-tight text-gray-900 sm:text-4xl">{{ $t('msgeight') }}</p>
            <p class="mx-auto mt-6 max-w-2xl text-lg leading-8 text-gray-600">
                {{ $t('msgnine') }}
            </p>
        </div>

        <div class="mt-20 max-w-lg sm:mx-auto md:max-w-none">
            <div class="grid grid-cols-1 gap-y-16 md:grid-cols-2 md:gap-x-12 md:gap-y-16">
                <div v-for="feature in features" :key="feature.name" class="realtive flex flex-col gap-6 sm:flex-row md:flex-col lg:flex-row">
                    <div class="flex h-12 w-12 items-center justify-center rounded-xl bg-indigo-100 text-white sm:shrink-0">
                        <img class="max-h-[30px]"  :src="feature.icon">
                    </div>
                    <div class="sm:min-w-0 sm:flex-1">
                        <p class="text-lg font-semibold leading-8 text-gray-900">{{ feature.name }}</p>
                        <p class="mt-2 text-base leading-7 text-gray-600">{{ feature. description }}</p>
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
                features : [
                    {
                        name: this.$t("msgtwtwo"),
                        description: this.$t("msgtwthree"),
                        icon: require("../assets/dollar.png"),
                    },
                    {
                        name: this.$t("msgtwtfr"),
                        description: this.$t("msgtwtfv"),
                        icon: require("../assets/activity.png"),
                    },
                    {
                        name: this.$t("msgtwtsix"),
                        description: this.$t("msgtwtsvn"),
                        icon: require("../assets/business.png"),
                    },
                    {
                        name: this.$t("msgtwteight"),
                        description: this.$t("msgtwtnin"),
                        icon: require("../assets/ecosystem.png"),
                    },
                ]
            }
        }
}

</script>

<style>

</style>