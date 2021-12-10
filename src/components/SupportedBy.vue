<template>
  <v-container fluid mx-0 pa-0 mt-5 class="all">
    <v-row justify="center" align="center">
      <v-col cols="lg-2 4">
        <v-img
          src="../assets/logo.png"
          contain
          height="70"
          justify="center"
        ></v-img>
      </v-col>
    </v-row>
    <v-row justify="center" align="center">
      <v-col cols="lg-3 4">
        <h2 class="text-center teks">Didukung Oleh</h2>
      </v-col>
    </v-row>
    <v-row justify="center" align="center">
      <v-img
        v-for="logo in logos"
        :key="logo"
        :src="require('../assets/' + logo)"
        contain
        height="100"
      >
      </v-img>
    </v-row>
  </v-container>
</template>

<style scoped>
.all {
  background-color: #f1f1f1;
}
.image {
  margin-top: 10%;
}
.teks {
  margin-top: -5%;
}
@media screen and (max-width: 991px) {
  .all {
    border-top-left-radius: 0;
  }
}
</style>

<script>
export default {
  name: "SupportedBy",
  data() {
    return {
      logos: ["1000.png", "chub.png"],
    };
  },
};
</script>
