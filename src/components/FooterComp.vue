<template>
  <div class="footer">
    <div class="footer-wrapp container">
        <div class="footer-logo">
            <img src="../assets/img/Frame 53.png" alt="">
        </div>
        <NavItems class="footer-items" textColor="white"></NavItems>
        <div class="footer-about">
            <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna</span>
        </div>
        <div class="footer-links">
            <FooterLinks></FooterLinks>
            <FooterLinks></FooterLinks>
            <FooterLinks></FooterLinks>
            <FooterLinks></FooterLinks>
        </div>
    </div>
  </div>
</template>

<script setup>
import NavItems from './ui/NavItems.vue'
import FooterLinks from './ui/FooterLinks.vue'
</script>

<style scoped>
    .footer {
        background: black;
        margin-top: 175px;
    }
    
    .footer-wrapp {
        padding-top: 124px;
        padding-bottom: 124px;
        display: grid;
        gap: 62px;
    }

    .footer-logo {
        text-align: center;
    }

    .footer-items {
        margin: 0 auto;
    }
    .footer-about {
        max-width: 709px;
        text-align: center;
        margin: 0 auto;
        color: white;
        opacity: 60%;
        font-size: 20px;
        line-height: 30px;
    }
    .footer-links {
        display: flex;
        justify-content: space-between;
        text-align: center;
    }
</style>