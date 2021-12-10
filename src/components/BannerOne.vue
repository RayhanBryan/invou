<template>
  <v-container class="all" fluid ma-0 pa-0>
    <v-row>
      <v-col cols="12">
        <v-img src="../assets/arrow.svg" width="5%" class="image"> </v-img>
        <h1>
          Membantu eventmu untuk dapat berkembang secara maksimal adalah misi
          utama kami.
        </h1>
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>
.all {
  background: linear-gradient(
    175deg,
    var(--secondary-color) 60%,
    var(--primary-color)
  );
  color: white;
  text-align: center;
}
.image {
  display: block;
  margin-left: auto;
  margin-right: auto;
  margin-top: 5%;
}
h1 {
  margin: 0 25% 5% 25%;
  font-weight: 300;
}

@media screen and (max-width: 991px) {
  h1 {
    font-size: 15px;
  }
}
</style>

<script>
export default {
  name: "BannerOne",
};
</script>
