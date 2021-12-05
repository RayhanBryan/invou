<template>
    <v-container class="container" fluid mx-0 pa-0>
        <v-row justify="center" class="text-center row">
            <v-col cols="lg-4 12">
                <v-card class="justify-center card pt-5" color="#F1F1F1">
                    <v-img
                        src= '../assets/connect1.png'
                        class="image"
                    >
                        
                    </v-img>
                    <v-card-title class="justify-center"> 
                        All-in-1 Database
                    </v-card-title>
                    <v-card-subtitle class="mb-1">
                        Pelajari preferensi pendanaan hingga jelajahi event potensial melalui database
                    </v-card-subtitle>
                    <v-card-action>
                    </v-card-action>
                </v-card>
                <v-btn
                    color="var(--secondary-color)"
                    class="mb-3 mt-5 justify-center"
                >
                    <span class="button-text">Pelajari Sekarang</span>
                </v-btn>
            </v-col>
            <v-spacer class="spacer"></v-spacer>
            <v-col cols="lg-4 12">
                <v-card class="justify-center card pt-5" color="#F1F1F1">
                    <v-img
                        src= '../assets/connect2.png' 
                        class="image"
                    >
                        
                    </v-img>
                    <v-card-title class="justify-center"> 
                        Ajukan Pendanaan
                    </v-card-title>
                    <v-card-subtitle>
                        Terhubung dengan entitas sponsor yang tepat dengan bergabung didalam ekosistem kami!
                    </v-card-subtitle>
                    <v-card-action>
                    </v-card-action>
                </v-card>
                <v-btn
                    color="var(--secondary-color)"
                    class="mb-3 mt-5 justify-center"
                >
                    <span class="button-text">Ajukan Sekarang</span>
                </v-btn>
            </v-col>
        </v-row>
    </v-container>
</template>

<style scoped>
    .container {
        background-image: url("../assets/bg-journey.png");
    }
    .card {
        margin-top: 10%;
    }
    .row {
        margin: 0 10%;
    }
    .button-text {
        color: white;
    }
    .banner {
        background-color: var(--secondary-color);
        margin: 0;
    }
    .image {
        height: 50%;
        margin: 20px;
    }

    @media screen and (max-width: 991px) {
        .spacer{
            display: none;
        }
    }
</style>

<script>
export default {
    name: 'ConnectUs',

    data(){
        return {
            items: [
                {
                    name: '',
                    text: '',
                    image: ''
                },
                {
                    name: '',
                    text: '',
                    image: '#'
                }

            ]

        }
    }
}
</script>