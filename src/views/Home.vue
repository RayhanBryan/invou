<template>
  <div class="ma-0">
    <the-jumbotron />
    <connect-us />
    <banner-one />
    <the-journey />
    <count-org />
    <our-event />
    <supported-by />
  </div>
</template>

<style scoped>

</style>

<script>
  import BannerOne from '../components/BannerOne.vue'
  import ConnectUs from '../components/ConnectUs.vue'
  import CountOrg from '../components/CountOrg.vue'
  import OurEvent from '../components/OurEvent.vue'
  import SupportedBy from '../components/SupportedBy.vue'
  import TheJourney from '../components/TheJourney.vue'
  import TheJumbotron from '../components/TheJumbotron.vue'

  export default {
    name: 'Home',

    components: {
        TheJumbotron,
        ConnectUs,
        BannerOne,
        TheJourney,
        CountOrg,
        OurEvent,
        SupportedBy
    },
  }
</script,
        SupportedBy>
