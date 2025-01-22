<template>

<div>
  <Navigation/>
  <Header/>
  <Skills/>
  <Gallery/>
  <Footer/>

  
</div>


</template>


<script>
import Navigation from './components/Navigation.vue';
import Footer from './components/Footer.vue';
import Header from './components/Header.vue';
import Skills from './components/Skills.vue';
import Gallery from './components/Gallery.vue';

export default {
  components:{
    Navigation,
    Footer,
    Header,
    Skills,
    Gallery
  }
}
</script>


<style scoped>
div{
  width: 1280px;
  margin: 0 auto;
}
</style>