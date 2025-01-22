<template>
    <section class="services">
    
      <div class="service" v-for="item in service" :key="item.id">
        <img :src="item.imgSrc" :alt="item.title + ' Icon'" />
        <h3>{{ item.title }}</h3>
        <p>{{ item.text }}</p>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    data() {
      return {
        service: [
          { id: 1, imgSrc: "../src/assets/service1.png", title: 'Product Design', text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com' },
          { id: 2, imgSrc: "../src/assets/service2.png", title: 'Visual Design', text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com' },
          { id: 3, imgSrc: "../src/assets/service3.png", title: 'Art Direction', text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com' }
        ]
      }
    }
  }
  </script>
  
  <style scoped>
  .services {
    width: 100%;
    height: 513px;
    display: flex;
    justify-content: space-around;
    align-items: flex-start;

    font-family: "Epilogue";

  }
  .service {
    width: 394px;
    text-align: center;
    height: 429px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 40px;
    color: #2D2D2D;
  }
  .service img {
    width: 124px;
    height: 124px;

  }
  .service h3 {
    margin-bottom: 10px;
    font-size: 27px;
    line-height: 42px;
    font-weight: 600;
  }
  .service p {
    font-size: 17px;
    line-height: 27px;
    font-weight: 400;
  }
  </style>