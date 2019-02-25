<template>
  <div>
  <h4 class="q-ma-xs q-pb-md">Featured</h4>
  <InfoCard/>
  </div>
</template>

<script>
import InfoCard from '../components/InfoCard'
export default {
  name: 'FeaturePage',
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

<style lang="stylus">
@import '~variables'

body
  background $primary

</style>
