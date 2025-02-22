<template>
  <div class="about-wrapp container">
    <div class="about-info">
        <div class="info-title">
            <h2>Your Trusted Partner in Cloud Technology</h2>
        </div>
        <div class="info-text">
            <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed deiusmod tempor incididunt ut labore et dolore magna</span>
        </div>
        <div class="info-pluses">
            <div class="pluses-body">
                <div class="pluses-title">
                    <h3>290+</h3>
                </div>
                <div class="pluses-text">
                    <span>Lorem ipsum dolor</span>
                </div>
            </div>
            <div class="pluses-body">
                <div class="pluses-title">
                    <h3>98%</h3>
                </div>
                <div class="pluses-text">
                    <span>Lorem ipsum dolor</span>
                </div>
            </div>
            <div class="pluses-body">
                <div class="pluses-title">
                    <h3>17K+</h3>
                </div>
                <div class="pluses-text">
                    <span>Lorem ipsum dolor</span>
                </div>
            </div>
        </div>
        <div class="info-btn">
            <ButtonComp class="about-btn">Get Started</ButtonComp>
        </div>
    </div>
    <div class="about-cards">
        <CardComp :show="false" class="card"></CardComp>
        <CardComp :show="false" class="card"></CardComp>
        <CardComp :show="false" class="card"></CardComp>
    </div>
  </div>
</template>

<script setup>
import CardComp from './ui/CardComp.vue'
import ButtonComp from './ui/ButtonComp.vue'
</script>
<style scoped>
.about-wrapp {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 175px;
}

.about-info {
    max-width: 719px;
    width: 100%;
    display: grid;
    gap: 74px;
}

.info-title h2 {
    font-size: 48px;
    font-weight: 500;
    line-height: 58.5px;
    text-transform: uppercase;
    letter-spacing: 1px;
}

.info-text span {
    font-size: 20px;
    opacity: 80%;
}

.card {
    max-width: 467px;
    width: 100%;
    height: 157px;
    display: flex;
    padding: 47px 67px;
}

.pluses-body {
    max-width: 192px;
    width: 100%;
    display: grid;
    gap: 9px;
}

.pluses-title h3 {
    font-size: 40px;
}

.pluses-text span {
    font-size: 20px;
    opacity: 80%;
}

.info-pluses {
    width: 100%;
    display: flex;
    justify-content: space-between;
}
.about-cards {
    display: grid;
    gap: 42px;
    margin-right: 5px;
}

.about-btn {
    max-width: 278px;
    width: 100%;
    height: 59px;
}
</style>