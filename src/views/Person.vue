<template>
  <v-card>
    <v-container grid-list-md text-xs-center>
      <v-layout row wrap>
        <v-flex v-for="person in persons" :key="person" xs4 d-flex>
          <img :src="person" />
        </v-flex>
      </v-layout>
    </v-container>
  </v-card>
</template>

<script>
export default {
  data: () => ({
    persons: [
      require("../assets/person/person01.jpg"),
      require("../assets/person/person02.jpg"),
      require("../assets/person/person03.jpg"),
      require("../assets/person/person04.jpg"),
      require("../assets/person/person05.jpg"),
      require("../assets/person/person06.jpg"),
      require("../assets/person/person07.jpg"),
      require("../assets/person/person08.jpg"),
      require("../assets/person/person09.jpg")
    ]
  })
};
</script>

<style></style>
