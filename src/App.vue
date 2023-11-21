<template>
  <div id="app">
   <landing-page/>
  </div>
</template>

<script>
import LandingPage from './components/LandingPage.vue';

export default {
  name: 'App',
  components:{
      LandingPage

  }
}
</script>

<style scoped>
 *{
  margin:0;
} 
div{
  height:100vh;
  margin:0;
}
#app{
  background-image:url(@/assets/background-home-desktop.jpg);
  height:100%;
  width:100%;
  margin:0;
}
@media (min-width:600px)and (max-width:1024px){
  #app{
    background-image: url(@/assets/background-home-tablet.jpg);
  }
}
@media (max-width:599px) {
  #app{
    background-image: url(@/assets/background-home-mobile.jpg);
  }
}
</style>
