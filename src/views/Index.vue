<template>
  <div class="index">
      <Carouset msg="swiper"/>
      <Roomtitle msg="roomtitle"/> 
      <Roomdescription :description="description" msg="Roomdescription"/>
      <Maps :maps="maps" msg="maps"/>
      <Listing :listing="listing" msg="listing" />
  </div>
</template>

<script>
import Carouset from '@/components/Carouset.vue'
import Roomtitle from '@/components/Roomtitle.vue'
import Roomdescription from '@/components/Roomdescription.vue'
import Maps from '@/components/maps.vue'
import Listing from '@/components/ListingDetails.vue'
export default {
  name: 'Index',
  components: {
    Carouset,
    Roomtitle,
    Roomdescription,
    Maps,
    Listing
  },
  data(){
　　 return {
      description:"Description",
      maps:"Location",
      listing:"ListingDetails"
    }
  }
}
</script>

<style lang="stylus" scoped>

</style>
