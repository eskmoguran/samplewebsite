<template>
  <v-app>
    <sideMenuItem />
    <headerItem />
    <v-content><router-view /></v-content>
    <footerItem />
  </v-app>
</template>

<script>
import headerItem from "./components/headerItem";
import footerItem from "./components/footerItem";
import sideMenuItem from "./components/sideMenuItem";

export default {
  name: "App",
  components: {
    headerItem,
    footerItem,
    sideMenuItem
  },
  data() {
    return {
      //
    };
  }
};
</script>
