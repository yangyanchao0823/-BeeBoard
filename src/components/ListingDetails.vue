<template>
  <div class="list">
      <p class="p1">{{listing}}</p>
      <p>La Verti Residences Tower,28 Great Sutton St,Bangkok,Thailand</p>
  </div>
</template>

<script>
export default {
  name: 'Listing',
  props: {
    msg: String,
    listing: String
  }
}
</script>

<style scoped lang="scss">
$border-color: #f2f2f2;
    .list{
    margin-top:15px ;
    width: 90%;
    margin-left:5% ;
    border-bottom:1px solid $border-color ;
    .p1{
      font-size:24px;
      font-weight: bold;
    }
}
</style>
