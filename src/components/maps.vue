
<template>
    <div class="mymap">
        <p class="p1">{{maps}}<p>
      <div id="map"></div>
    </div>
</template>

<style scoped>
.mymap{
width: 90%;
margin-left:5%;
margin-top:10px;
border-bottom:1px solid #f2f2f2 ;
}
.p1{
font-size:24px;
font-weight: bold;
}
#map{
width:100%;
height:200px;
margin-bottom:20px ;
}
</style>

<script>
    export default {
        name: 'Maps',
        props: {
            msg: String,
            maps: String
        },
      data(){
          return{
            
          }
      },
      created(){
        //页面刚进入时开启长连接
        // this.initWebSocket()
      },
      destroyed: function() {
        //页面销毁时关闭长连接
        this.websocketclose();
      },
      mounted(){
      this.mapBuild() //初始化实例之后调用
      },
      methods:{
        //  地图实例
        mapBuild(){
            let myLatLng = {lat: -25.363, lng: 131.044};

  　　　 　  let map = new google.maps.Map(document.getElementById('map'), {
    　　　　　　zoom: 4,
    　　　　　　center: myLatLng
  　　　　　    });

  　　　　　let marker = new google.maps.Marker({
    　　　　　　position: myLatLng,
    　　　　　　map: map,
    　　　　　　title: 'Hello World!'
 　　　　　});
        },
      },
    }
</script>