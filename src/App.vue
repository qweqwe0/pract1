<template>

<div>
  <Navigation/>
  <Footer/>
</div>



</template>


<script>
import Navigation from './components/Navigation.vue';
import Footer from './components/Footer.vue';

export default {
  components:{
    Navigation,
    Footer
  }
}
</script>


<style scoped>
div{
  width: 1280px;
  margin: 0 auto;
}
</style>