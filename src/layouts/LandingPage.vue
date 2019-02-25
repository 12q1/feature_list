<template>
  <div>
  <h3>Featured</h3>
  <div>
  <InfoCard/>
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

<style lang="stylus" scoped>
@import '~variables'
</style>
