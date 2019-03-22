<template>
  <v-navigation-drawer :clipped="$vuetify.breakpoint.lgAndUp" fixed app>
    <v-toolbar flat>
      <v-list>
        <v-list-tile>
          <v-list-tile-title class="title">
            メニュー
          </v-list-tile-title>
        </v-list-tile>
      </v-list>
    </v-toolbar>
    <v-divider></v-divider>
    <ul>
      <div class="text-xs-center">
        <v-btn round color="primary" dark @click="movePage('person')">人物</v-btn>
      </div>
      <div class="text-xs-center">
        <v-btn round color="primary" dark @click="movePage('animal')">動物</v-btn>
      </div>
      <div class="text-xs-center">
        <v-btn round color="primary" dark>風景</v-btn>
      </div>
      <div class="text-xs-center">
        <v-btn round color="primary" dark>料理</v-btn>
      </div>
    </ul>
  </v-navigation-drawer>
</template>

<script>
export default {
    methods: {
        movePage(link){
            this.$router.push(link)
        }
    }
}
</script>

