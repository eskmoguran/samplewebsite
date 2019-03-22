<template>
  <v-card>
    <v-container grid-list-md text-xs-center>
      <v-layout row wrap>
        <v-flex v-for="animal in animals" :key="animal" xs4 d-flex>
          <img :src="animal" />
        </v-flex>
      </v-layout>
    </v-container>
  </v-card>
</template>

<script>
export default {
  data: () => ({
    animals: [
      require("../assets/animal/animal01.jpg"),
      require("../assets/animal/animal02.jpg"),
      require("../assets/animal/animal03.jpg"),
      require("../assets/animal/animal04.jpg"),
      require("../assets/animal/animal05.jpg"),
      require("../assets/animal/animal06.jpg"),
      require("../assets/animal/animal07.jpg"),
      require("../assets/animal/animal08.jpg"),
      require("../assets/animal/animal09.jpg")
    ]
  })
};
</script>

<style></style>
