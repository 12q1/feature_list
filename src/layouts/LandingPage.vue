<template>
  <div>
  <h3>Featured</h3>
  <div class="container">
  <InfoCard :items="items"/>
  </div>
  </div>
</template>

<script>
import InfoCard from '../components/InfoCard'
export default {
  name: 'LandingPage',
  components: {
    InfoCard
  },
  data () {
    return {
      items: []
    }
  }
}
</script>

<style>

h3 {
  font-size: 25px;
  padding: 15px;
}

.container {
  display: flex;
  flex-direction: row;
}

</style>
