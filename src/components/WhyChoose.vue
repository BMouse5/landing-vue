<template>
  <div class="why-wrapp container">
    <div class="why-header">
        <CardComp :show="true"></CardComp>
        <CardComp :show="true"></CardComp>
        <CardComp :show="true"></CardComp>
    </div>
    <div class="why-body">
        <div class="why-title">
            <div class="title-text">
                <h2>Why choose us</h2>
            </div>
            <div class="title-about">
                <span>Lorem ipsum dolor sit amet, conctetur adipiscing elit, sed do eiusmod </span>
            </div>
            <div class="title-btn">
                <ButtonComp>Contact us</ButtonComp>
            </div>
        </div>
        <div class="why-about">
            <div class="about-text">
                <h1>Experience, Reliability, and Innovation in Every Cloud Solution</h1>
            </div>
        </div>
    </div>
  </div>
</template>

<script setup>
import CardComp from './ui/CardComp.vue'
import ButtonComp from './ui/ButtonComp.vue'
</script>
<style scoped>
.why-header {
    display: flex;
    justify-content: space-between;
    margin-top: 175px;
}

.why-body {
    display: flex;
    justify-content: space-between;
    margin-top: 152px;
}

.why-title {
    display: grid;
    gap: 40px;
}

.title-text {
    max-width: 258px;
    height: 98px;
}

.title-text h2 {
    font-size: 40px;
    font-weight: 500;
    text-transform: uppercase;
}

.title-about {
    max-width: 399px;
    width: 100%;
    height: 60px;
}

.title-about span {
    font-size: 20px;
    font-weight: 400;
    opacity: 80%;
    color: #0E0E0E;
    line-height: 30px;
}

.why-about {
    max-width: 752px;
    width: 100%;
    height: 312px;
}
.about-text h1 {
    font-size: 61px;
    line-height: 78px;
    letter-spacing: 4px;
}
</style>