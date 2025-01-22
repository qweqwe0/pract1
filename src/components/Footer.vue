<template>

<footer>
    <div class="footer-cont">
        <h2>Lets work together</h2>
        <div class="contact-section">
            <div class="contact-info">
                <p>
                    This is a template Figma file, turned into code using Anima.
                     Learn more at AnimaApp.com This is a template Figma file, 
                     turned into code using Anima. Learn more at AnimaApp.com
                </p>
                <div class="social-links">
                    <a href="https://discord.com/invite/eQxkYTNxSp"><img :src="discord" alt="discord"></a>
                    <a href="https://www.facebook.com/animaapp/"><img :src="facebook" alt="facebook"></a>
                    <a href="https://dribbble.com/animaapp"><img :src="dribbble" alt="dribbble"></a>
                    <a href="https://www.instagram.com/animaapp/?hl=en"><img :src="instagram" alt="instagram"></a>
                    <a href="https://www.behance.net/Anima_design"><img :src="behance" alt="behance"></a>
                </div>
            </div>
            <form class="contact-form">
                <div class="input-field">
                    <input type="text" placeholder="Name">
                    <input type="email" placeholder="Email">
                </div>
                <button>Submit</button>
            </form>
        </div>
    </div>
</footer>
   
</template>

<script>
import discord from '../assets/discord.png'
import facebook from '../assets/facebook.png'
import dribbble from '../assets/dribbble.png'
import instagram from '../assets/nstagram.png'
import behance from '../assets/behance.png'

export default{
    data(){
        return{
            discord: discord,
            facebook: facebook,
            dribbble: dribbble,
            instagram: instagram,
            behance: behance

        }
    }
}
</script>

<style scoped>
footer{
    height: 426px;
    width: 100%;
    color: #2D2D2D;
}
.footer-cont{
    font-family: "Epilogue";
    display: flex;
    flex-direction: column;
    margin-left:30px ;
    margin-right:30px ;
}
h2{
    font-size: 32px;
    font-weight: 600;
}
.contact-section{
    height: 232px;
    display: flex;
    justify-content: space-between;
}
.contact-info{
    width: 570px;
    height: 159px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}
.contact-info p{
    font-size: 17px;
    font-weight: 400;
    line-height: 27px;
}
.social-links{
    display: flex;
    gap: 15px;
}
.social-links img{
    width: 36px;
    height: 36px;
}
.contact-form{
    width: 520px;
    height: 232px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}
.input-field{
    width: 520px;
    height: 130px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}
input {
    width: 515px;
    height: 50px;
    font-size: 17px;
    background-color: #F3F3F3;
    border: none;
}
button{
    width: 199px;
    height: 78px;
    color: white;
    background-color: #2D2D2D;
    font-size: 20px;
}
</style>

