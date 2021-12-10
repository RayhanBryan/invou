<template>
  <v-container fluid mx-0 pa-0 class="all">
    <v-row align="center" justify="center">
      <h1>Pelatihan Event Terdekat</h1>
    </v-row>
    <v-row align="center" justify="center" class="text-center">
      <p>Tingkatkan kapabilitas timmu melalui seri pelatihan online</p>
    </v-row>

    <v-row>
      <v-sheet class="mx-auto" max-width="100%" justify="center" align="center">
        <v-slide-group v-model="model" class="pa-4" show-arrows>
          <v-slide-item
            v-for="event in events"
            :key="name in event"
            v-slot="{ active, toggle }"
          >
            <v-card
              :to="event.to"
              color="white"
              class="ma-4"
              height="500"
              width="300"
            >
              <v-row>
                <v-img
                  :src="require('../assets/' + event.image)"
                  width="280"
                  class="ma-5"
                ></v-img>
              </v-row>
              <v-row align="center">
                <h1 class="ml-5">{{ event.name }}</h1>
              </v-row>

              <v-row>
                <p class="ml-5 mt-2 mr-5">{{ event.text }}</p>
              </v-row>

              <v-row>
                <v-card-actions class="act">
                  <v-btn text color="var(--primary-color)">
                    <h5>Daftar</h5>
                  </v-btn>
                </v-card-actions>
              </v-row>
            </v-card>
          </v-slide-item>
        </v-slide-group>

        <v-expand-transition>
          <v-sheet v-if="model != null" height="200" tile>
            <v-row class="fill-height" align="center" justify="center">
              <h3 class="text-h6">Selected {{ model }}</h3>
            </v-row>
          </v-sheet>
        </v-expand-transition>
      </v-sheet>
    </v-row>
  </v-container>
</template>

<style scoped>
.all {
  margin-top: 5%;
}
.v-card h1 {
  font-size: 24px;
  text-align: left;
}
.v-card p {
  text-align: left;
}
.act {
  position: absolute;
  left: 1px;
  bottom: 0;
}
h5 {
  font-size: 15px;
}
</style>

<script>
export default {
  name: "OurEvent",

  data() {
    return {
      events: [
        {
          name: "Sharing Session #1",
          text: "Pelajari kiat-kiat perencanaan event bersama mentor praktisi profesional!",
          image: "event1.png",
          to: "",
        },
        {
          name: "Sharing Session #1",
          text: "Ngobrol bareng seputar volunteering dan cara mendapatkan beasiswa volunteeer fully-funded!",
          image: "event2.png",
        },
        {
          name: "Sharing Session #1",
          text: "Pelajari kiat-kiat perencanaan event bersama mentor praktisi profesional!",
          image: "event1.png",
        },
        {
          name: "Sharing Session #1",
          text: "Pelajari kiat-kiat perencanaan event bersama mentor praktisi profesional!",
          image: "event2.png",
        },
        {
          name: "Sharing Session #1",
          text: "Pelajari kiat-kiat perencanaan event bersama mentor praktisi profesional!",
          image: "event1.png",
        },
        {
          name: "Sharing Session #1",
          text: "Pelajari kiat-kiat perencanaan event bersama mentor praktisi profesional!",
          image: "event2.png",
        },
      ],
      model: null,
    };
  },
};
</script>
