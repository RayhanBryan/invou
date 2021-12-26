<template>
    <v-container class="all" fluid my-0 py-0>
        <v-row class="text-center">
            <v-col>
                <h1>PELAJARI EKOSISTEM INVOU DALAM ANGKA</h1>
            </v-col>
        </v-row>
        <v-row>
            <v-col
                class="fluid"
                v-for="item in items" :key="title in item"
            >
                <v-row
                    align="center"
                    justify="center"
                
                >
                    <h2> {{ item.count }} </h2>
                </v-row>
                <v-row
                    align="center"
                    justify="center"
                    class="text-center"
                >
                    <h5> {{ item.title }} </h5>
                </v-row>
            </v-col>
        </v-row>
    </v-container>
</template>

<style scoped>
    .all {
        background: black;

    }

    h1 {
        color: white;
        font-size: 30px;
    }

    h2 {
        color: white;
        font-size: 150px;
        margin-top: 30%;
    }

    h5 {
        color: white;
        font-size: 20px;
        margin-top: -10%;
        margin-bottom: 50%;
    }

@media screen and (max-width: 991px) {
    .all {
        border-top-left-radius: 0;
    }
    h2 {
        font-size: 100px;
    }
    h5 {
        font-size: 10px;
    }
}
</style>

<script>
export default {
    name: 'CountOrg',

    data(){
        return {
            items: [
                {
                    title: 'Event Organizer',
                    count: 1,
                },
                {
                    title: 'Organisasi',
                    count: 3,

                },
                {
                    title: 'Pelatihan Event Terlaksana',
                    count: 2,

                },
                {
                    title: 'Seri Mini Podcast',
                    count: 6,

                }

            ],
            countdown: 0,

        }
    },

    // methods: {
    //     countSeconds() {
    //                     for (const a in this.items){
    //                         var b = this.items[a].count
    //                         this.items[a].count = 0
    //                         if(this.items[a].count < 10) {
    //                             setTimeout(() => {
    //                                 this.items[a].count+= 1
    //                                 this.countSeconds()
    //                             }, 500);
    //                         }
    //                     }
    //     }
    // },
    //     created() {
    //         this.countSeconds();
    //     }

    // methods: {
    //     countSeconds() {
    //                     if(this.countdown> 0) {
    //                         setTimeout(() => {
    //                             this.countdown += 1
    //                             this.countSeconds()
    //                         }, 500);
    //                     }
    //                 }
    //     },
    //     created() {
    //         this.countSeconds();
    //     }
}
</script>