<template>
  <div>
  <p>Featured</p>
  <InfoCard/>
  <div v-for="(item, index) of items" :key="index">
    <p>{{ item }}</p>
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
      items: [{ title: 'Kira', subtitle: `It's How You Know What's In Your Contracts`, avatar: `kira.jpg`, description: `Kira is a powerful machine learning software that identifies, extracts and analyzes text in your contracts and other documents` }, { title: 'Doxly', subtitle: `Secure Portal for End to End Transactions`, avatar: `doxly.jpg`, description: `Manage the entire legal transaction process from dilligence to closing` }, { title: 'Clause', subtitle: `Connected Contracting`, avatar: `clause.jpg`, description: `Clause builds the technology infrastructure for connected contracts to increase the vlaue and improve the management of your business agreements` }]
    }
  }
}
</script>

<style>
</style>
