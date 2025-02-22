<template>
  <div class="testimonial-wrapp">
    <div class="testimonial-title">
        <h1>Our Clients’ Success Speaks for Itself</h1>
        <img src="../assets/img/format_quote.png" alt="">
    </div>
    <div class="slider-wrapp">
        <SliderComp></SliderComp>
    </div>
  </div>
</template>

<script setup>
import SliderComp from './ui/SliderComp.vue'
</script>

<style scoped>
.testimonial-wrapp {
    max-width: 1322px;
    width: 100%;
    margin: 0 auto;
    margin-top: 175px;
}

.testimonial-title {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.testimonial-title h1 {
    font-size: 59px;
    max-width: 598px;
    width: 100%;
    line-height: 78px;
}

.testimonial-title img {
    opacity: 10%;
}
</style>