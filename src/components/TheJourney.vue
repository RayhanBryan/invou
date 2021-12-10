<template>
  <v-container fluid mx-0 pa-0 class="all">
    <v-row>
      <v-col>
        <v-img src="../assets/journey1.png" class="image1"> </v-img>
      </v-col>
      <v-col align-self="center">
        <div class="text1 fluid">
          <p>KEBUTUHANMU ADA DI SINI</p>
          <h2>Database Sponsor, Database Organisasi, dan Pelatihan Event</h2>
          <p>
            Kembangkan organisasimu dengan akses untuk mempelajari ekosistem
            event di Indonesia melalui database tervalidasi hingga pengembangan
            kapabilitas tim dengan pelatihan event dua arah maupun satu arah.
          </p>
        </div>
      </v-col>
    </v-row>
    <v-row>
      <v-col align-self="center">
        <div class="text2 fluid">
          <p>EKOSISTEM PENDANAAN EVENT</p>
          <h2>Bergabung Kedalam Ekosistem Event Invou!</h2>
          <p>
            Daftarkan organisasimu kedalam ekosistem Invou dan dapatkan
            kesempatan untuk mendapaatkan pendanaan sponsorship.
          </p>

          <v-btn color="var(--secondary-color)" class="justify-center">
            <h5 class="text-btn">Gabung Invou!</h5>
          </v-btn>
        </div>
      </v-col>
      <v-col>
        <v-img src="../assets/journey2.png" class="image2"> </v-img>
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <v-img src="../assets/journey3.png" class="image3"> </v-img>
      </v-col>
      <v-col align-self="center">
        <div class="text1 fluid">
          <p>PENDANAAN TANPA RIBET</p>
          <h2>Menjodohkanmu dengan Sponsorship yang Tepat</h2>
          <p>
            Kami akan mengkurasi dan mereview setiap proposal event yang telah
            bergabung dalam ekosistem Invou. Setelah proses kurasi yang ketat,
            event kalian akan mendapatkan pendanaan dari sponsor yang tepat.
          </p>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>
.all {
  margin-top: 10px;
  background-image: url("../assets/bg-journey.png");
}

.image1 {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 50%;
}
.text1 {
  margin-right: 20%;
}

.text2 {
  margin-left: 10%;
}
.text-btn {
  color: white;
}
.image2 {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 50%;
}

.image3 {
  display: block;
  margin-left: auto;
  margin-right: auto;
  margin-bottom: 10px;
  width: 50%;
}

.break1 {
  margin-top: 2%;
  color: var(--secondary-color);
  height: 2px;
}

@media screen and (max-width: 767px) {
  .all {
  }
  .text1 {
    text-align: center;
    margin: auto;
  }
  .text2 {
    position: relative;
    top: 210px;
    text-align: center;
    margin: auto;
  }
  .image2 {
    position: relative;
    bottom: 270px;
  }
  .break1 {
    margin-bottom: 50px;
    color: var(--secondary-color);
    height: 2px;
  }
}
</style>

<script>
export default {
  name: "TheJourney",
};
</script>
