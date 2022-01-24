<template>
  <div class="search-box">
    <input id="myInput" type="search" placeholder="Search.." v-model="query" v-on:click="fetchWeather" />
  </div>

  <div class="weather-wrap">
    <div class="location-box">
      <div class="location">California, US
      </div>
      <div class="date">24 Jan, 2022</div>
    </div>
  </div>

  <div class="weather-box">
    <div class="temp">10°C</div>
    <div class="weather">Clouds
    </div>
  </div>



</template>

<script>

export default {
  name: 'App',
 data(){
   return{
     
   }
 }
}
</script>

<style>
body{
  background: #b6b6b6;
}
#app {
  font-family: System-ui;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;

}
#myInput{
  width: 90%;
  padding: 15px;

  border: none;
  background: rgba(245, 245, 245, 0.514);
  font-size: 22px;
  border-radius: 20px ;
  
}
.weather-wrap{
  margin: 50px;
}
.location-box{
  font-size: 30px;
  font-weight: bold;
}
.weather-box{
  text-align: center;
  margin: 10%;
  font-size: 30px;
  font-weight: bold;
}
.temp{
  margin-bottom: 50px;
  background: rgba(255, 255, 255, 0.438);
  align-content: center;
  padding:  70px 50px;
  margin: 30px;
  text-align:center;
  border-radius: 20px;
  font-size: 70px;
}

</style>
