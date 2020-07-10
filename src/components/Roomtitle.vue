<template>
  <div class="roomtitlediv">
      <p class="p1">$<i>{{num}}</i></p>&nbsp;<i>4</i>bds | <i>2</i>ba | <i>2,000</i>sqm
      <div><van-icon name="location" /><p class="p2">La Verti Residences Tower,28 Great Sutton St,Bangkok,Thailand</p></div>
      <div class="roomtitledivboot"><div class="yuan"></div><p  class="p3">Condo for sale</p></div>
  </div>
</template>

<script>
import axios from 'axios'
export default {
  name: 'Roomtitle',
  props: {
    msg: String 
  },
  data( ){
      return{
          num:"666.120.000"
      }
  }
}
</script>

<style scoped lang="scss">
$border-color: #f2f2f2;
.roomtitlediv{
    margin-top:15px ;
    width: 90%;
    margin-left:5% ;
    border-bottom:1px solid $border-color ;
    .p1{
      font-size:24px;
      font-weight: bold;
      display: inline;
    }
}
.roomtitlediv{
    i{
       font-style: normal; 
    }
}
.p2{
  display: inline;
}
.p3{
  display: inline;
}
.yuan{
  width: 11px;
  height: 11px;
  margin-top:3px ;
  margin-right:7px ;
  border-radius:50% ;
  background: #ff77e0;
  float: left;
}
.roomtitledivboot{
  margin-top:12px ;
  margin-bottom:20px ;
}
</style>
