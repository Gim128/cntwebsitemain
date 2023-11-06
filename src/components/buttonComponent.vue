<template>
  <div class="text-center">
      <v-menu data-app offset-y>
        <template v-slot:activator="{ on, attrs }">
          <v-btn
            data-app
            color="#0652DD"
            dark
            v-bind="attrs"
            v-on="on"
            type="button"
            style="min-width: 134px; height: 36px; padding: 0 6px;"
          >
            
            {{ $t("msgsxtthree") }}
          </v-btn>
        </template>
        <v-list data-app class="list">
          <v-list-item data-app
          @click="changelg(item.locale)"
            v-for="(item, index) in items"
            :key="index"
          >
            <v-list-item-title data-app>{{ item.title }}</v-list-item-title>
          </v-list-item>
        </v-list>
       </v-menu>
    </div>
</template>

<script>
export default {
  name: "ButtonView",

  methods: {
    changelg(locale){
      this.$i18n.locale = locale
      // location.reload()
    }
  },

  data: () => ({
    items: [
      { title: 'English' , locale: 'en' },
      { title: 'Chinese', locale: 'cn' },
    ],
  }),
}
</script>

<style>
  .list{
    min-width: 116px;
    top: 36px;
    left: 0px;
    transform-origin: left top;
    z-index: 101;
  }
</style>