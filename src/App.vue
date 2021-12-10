<template>
  <v-app>
    <v-app-bar app color="black" dark>
      <div class="d-flex align-center">
        <v-img
          alt="Invou Logo"
          class="shrink mr-2 logo"
          contain
          src="./assets/logo2.png"
          transition="scale-transition"
          width="120"
        />
      </div>

      <v-spacer></v-spacer>
      <v-btn href="" text>
        <span class="mx-1">Tentang Kami</span>
      </v-btn>
      <v-btn href="" text>
        <span class="mx-1">Cari Dana</span>
      </v-btn>
      <v-btn href="" text>
        <span class="mx-1">Beri Dana</span>
      </v-btn>
    </v-app-bar>

    <v-main>
      <router-view />
    </v-main>

    <v-container fluid mx-0 pa-0 class="all">
      <v-row align="center" justify="center" class="row-footer">
        <h1>Jadi <span>Bagian</span> dari Ekosistem <span>Invou</span>!</h1>
      </v-row>
      <v-row align="center" justify="center">
        <v-btn color="var(--secondary-color)">
          <h4>Hubungi Kami</h4>
        </v-btn>
      </v-row>
    </v-container>

    <v-container fluid mx-0 py-0 class="all2">
      <br />
      <br />
      <br />
      <v-row mt-5>
        <v-col cols="lg-5 sm-12" mt-5>
          <img src="./assets/logo.png" alt="" />
          <p>
            Invou merupakan platform event enabler. Kami berusaha membangun
            ekosistem pendanaan event yang baik di Indonesia melalui database
            tervalidasi dan menghubungkan organisasi dengan perusahaan sponsor.
          </p>
        </v-col>
        <v-col cols="lg-4 sm-12" mt-5>
          <h3>Produk Invou</h3>
          <v-list class="list">
            <v-list-item-group v-model="selectedItem" color="primary">
              <v-list-item v-for="(item, i) in items" :key="i">
                <v-list-item-icon>
                  <v-icon v-text="item.icon"></v-icon>
                </v-list-item-icon>
                <v-list-item-content>
                  <v-list-item-title v-text="item.text"></v-list-item-title>
                </v-list-item-content>
              </v-list-item>
            </v-list-item-group>
          </v-list>
        </v-col>
        <v-col cols="lg-3 sm-12" mt-5>
          <h3>Partner Utama</h3>
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<style>
:root {
  --primary-color: #00aeef;
  --secondary-color: #1c75bc;
}
.logo {
  margin-left: 55px;
}
</style>

<style scoped>
.all {
  margin-top: 10px;
  background: black;
  height: 150px;
}
h1 {
  margin-top: 40px;
  color: white;
  margin-bottom: 10px;
}

h1 span {
  color: var(--secondary-color);
}

h4 {
  color: white;
}

.all2 {
  background-color: #f1f1f1;
  padding: 0 100px !important;
}
.list {
  background-color: #f1f1f1 !important;
}
h3 {
  margin-left: 5%;
}
img {
  height: 50px;
}

@media screen and (max-width: 991px) {
  .all2 {
    padding: 0 20px !important;
  }

  h1 {
    font-size: 22px;
  }
}
</style>

<script>
export default {
  name: "App",

  data: () => ({
    items: [
      {
        icon: "mdi-account-group-outline",
        text: "Database Event",
      },
      {
        icon: "mdi-cash-multiple",
        text: "Database Sponsor",
      },
      {
        icon: "mdi-hand-heart",
        text: "Penyaluran Pendanaan",
      },
      {
        icon: "mdi-account-hard-hat",
        text: "Pelatihan Persiapan Event",
      },
    ],
  }),
};
</script>
