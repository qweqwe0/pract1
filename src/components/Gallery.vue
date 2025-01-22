<template>

<div class="gallery-section">
    <h2>Latest work</h2>
    <div class="cards-section">
        <div class="card" v-for="item in work" :key="work.id" >
            <img :src="item.imgSrc" :alt="item.id + 'work'"/>
            <div class="card-description">
                <h5>{{ item.title }} </h5>
                <p> {{ item.text }}</p>
            </div>
           
        </div>
    </div>
</div>

</template>



<script>

export default {
    data() {
      return {
        work: [
          { id: 1, imgSrc: "../src/assets/work1.png", title: 'Project title', text: 'UI, Art drection' },
          { id: 2, imgSrc: "../src/assets/work2.png", title: 'Project title', text: 'UI, Art drection' },
          { id: 3, imgSrc: "../src/assets/work3.png", title: 'Project title', text: 'UI, Art drection' },
          { id: 4, imgSrc: "../src/assets/work4.png", title: 'Project title', text: 'UI, Art drection' },
          { id: 5, imgSrc: "../src/assets/work5.png", title: 'Project title', text: 'UI, Art drection' },
          { id: 6, imgSrc: "../src/assets/work6.png", title: 'Project title', text: 'UI, Art drection' }
        ]
      }
    }
  }

</script>



<style scoped>

.gallery-section{
    width: 100%;
    height: 1030px;
    display: flex;
    flex-direction: column;
    align-items: center;
    color: #2D2D2D;
    font-family: "Epilogue";
    justify-content: space-around;
}
.cards-section{
    width: 1232px;
    height: 862px;
    display: grid;
    grid-template-columns: repeat(3,1fr);
    
    gap: 17px;
}
h2{
    font-size: 32px;
    line-height: 42px;
    font-weight: 600;
}
.card{
    display: flex;
    flex-direction: column;
    width: 395px;
    height: 419px;

}
.card-description {
    margin-top: 14px;
}
h5 {
    font-size: 20px;
    line-height: 30px;
    font-weight: 600;
    margin: 0 0 8px 0;
    
}

p {
    margin-top: -5px;
  font-size: 17px;
  line-height: 27px;
  color: #6d6d6d;
}

</style>