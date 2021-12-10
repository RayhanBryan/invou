<template>
  <v-container fluid class="pa-0 mx-0">
    <v-img class="image" src="../assets/header.png">
      <v-row>
        <v-col cols="lg-6 12">
          <h1
            data-aos="zoom-in-right"
            data-aos-duration="2000"
            data-aos-easing="ease-in-sine"
          >
            MENGHUBUNGKAN <span>EVENT</span> DENGAN <span>SPONSOR</span>
          </h1>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="12">
          <h3>
            Kami berusaha menghadirkan ekosistem pendanaan event melalui
            database tervalidasi dan akses kepada entitas sponsor
          </h3>
        </v-col>
      </v-row>
    </v-img>
  </v-container>
</template>

<style scoped>
.image {
}
h1 {
  margin-top: 10%;
  margin-left: 10%;
  color: white;
  font-size: 70px;
}
h1 span {
  color: var(--primary-color);
}
h3 {
  margin-right: 5%;
  margin-left: 5%;
  color: white;
  font-weight: 100;
  font-size: 25px;
}

@media screen and (max-width: 991px) {
  h1 {
    font-size: 30px;
    text-align: center;
    margin: 10% auto;
  }
  h3 {
    margin-top: -15%;
    margin-bottom: 15%;
    font-size: 20px;
    text-align: center;
  }
}
</style>

<script>
export default {
  name: "TheJumbotron",
};
</script>
