<template>

<div class="testimonial-section">
    <h2>Testimonial</h2>
    <div class="cards-container">
        <div class="card" v-for="item in client" :key="client.id">
            <p id="card-text">{{ item.text }}</p>
            <div class="client-info-cont">
                <img id="client-icon" :src="item.imgSrc" :alt="item.name">
                <div class="client-info">
                    <img id="stars" :src="item.stars">
                    <p id="name">{{ item.name }}</p>
                    <p id="company">{{ item.company }}</p>
                </div>
            </div>
        </div>
    </div>
</div>

</template>


<script>
export default {
    data() {
      return {
        client: [
          { id: 1, imgSrc: "../src/assets/clientIcon.png", text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com', stars: "../src/assets/stars.png", name: 'Gemma Nolen', company: 'Google' },
          { id: 2, imgSrc: "../src/assets/clientIcon.png", text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com', stars: "../src/assets/stars.png", name: 'Gemma Nolen', company: 'Google' },
          { id: 3, imgSrc: "../src/assets/clientIcon.png", text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com', stars: "../src/assets/stars.png", name: 'Gemma Nolen', company: 'Google' },
          { id: 4, imgSrc: "../src/assets/clientIcon.png", text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com', stars: "../src/assets/stars.png", name: 'Gemma Nolen', company: 'Google' },
          { id: 5, imgSrc: "../src/assets/clientIcon.png", text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com', stars: "../src/assets/stars.png", name: 'Gemma Nolen', company: 'Google' },
          { id: 6, imgSrc: "../src/assets/clientIcon.png", text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com', stars: "../src/assets/stars.png", name: 'Gemma Nolen', company: 'Google' }

        ]
      }
    }
  }
</script>



<style scoped>

.testimonial-section{
    color: #2D2D2D;
    font-family: "Epilogue";
    width: 100%;
    height: 852px;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    align-items: center;
}
h2{
    font-size: 32px;
    line-height: 42px;
    font-weight: 600;
}
.cards-container{
    width: 1232px;
    height: 684px;
    display: grid;
    grid-template-columns: repeat(3,1fr);
    gap: 24px;

}
#card-text{
    width: 310px;
    height: 90px;
    font-size: 20px;
    line-height: 30px;
    font-weight: 600;
}
.card{
    width: 395px;
    height: 330px;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    align-items: center;
    background-color: #F3F3F3;
}
.client-info-cont{
    width: 311px;
    height: 88px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}
#client-icon{
    width: 50px;
    height: 50px;
}
.client-info{
    width: 245px;
    height: 88px;
}
#stars{
    width: 120px;
    height: 20px;
}
#name{
    font-size: 20px;
    font-weight: 600;
}
#company{
    margin-top: -14px;
    font-size: 17px;
    font-weight: 400;

}

</style>