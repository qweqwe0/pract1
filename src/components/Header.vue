<template>


    
    <section class="header-section">
      <div class="header-content">
        <h2>Branding | Image making</h2>
        <h1>Visual Designer</h1>
        <p>This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com</p>
        <button>Contact</button>
      </div>
      <div class="hero-image">
        <img :src="HeaderImage" alt="Visual Designer" />
      </div>
    </section>

    <section class="logos">
      <img src="../assets/google.png" alt="Google" />
      <img src="../assets/nike.png" alt="Nike" />
      <img src="../assets/samsung.png" alt="Samsung" />
      <img src="../assets/apple.png" alt="Apple" />
      <img src="../assets/adidas.png" alt="Adidas" />
    </section>


   


</template>

<script>
import HeaderImage from '../assets/HeaderImage.png'

export default {
    data(){
        return{
            HeaderImage: HeaderImage,

        }
    }
}
</script>


<style scoped>
.header-section {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 60px;
  font-family: "Epilogue";
}
.header-content {
  max-width: 50%;
}
.header-content h2 {
 font-size: 20px;
 color: #2D2D2D;
 font-weight: 600;
}
.header-content h1 {
  margin: 10px 0;
  font-size: 68px;
  font-weight: 600;
  color: #2D2D2D;
}
.header-content p {
  margin: 20px 0;
  color: #2D2D2D;
  font-size: 17px;
  font-weight: 400;
  line-height: 27px;
}
.header-content button {
  margin-top: 10px;
  width: 211px;
  height: 78px;
  background-color: #2D2D2D;
  color: #fff;
  border: none;
  font-family: "Epilogue";
  font-size: 20px;
  line-height: 30px;
  font-weight: 600;
}
.header-image img {
  width: 100%;
  max-width: 400px;
  border-radius: 10px;
}

.logos {
  display: flex;
  justify-content: space-around;
  align-items: center;
  padding: 20px;
  background-color: #fff;
}



</style>