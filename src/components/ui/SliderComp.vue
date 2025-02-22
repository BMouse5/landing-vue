<template>
  <div class="slider">
    <div class="slider-picker">
        <button @click="previous">&lt;</button>
        <button @click="next">&gt;</button>
    </div>
    <div class="slider-body">
        <div class="body-quote">
            <span>"Scalable Solutions for a Growing Business"</span>
            <transition name="fade-slide" mode="out-in">
                <h3 :key="currentSlide">{{ slides[currentSlide] }}</h3>
            </transition>
        </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const currentSlide = ref(0);

const slides = [
    "Switching to [Cloud System’s Name] transformed our business operations. The seamless integration and excellent support team have empowered us to work faster and smarter. It’s the best decision we’ve made for our IT infrastructure!",
    "Our migration to the cloud was seamless, and we now have unmatched scalability and security. Couldn’t be happier with our decision!",
    "With [Cloud System’s Name], we reduced costs and improved efficiency across all departments. Highly recommended!"
]

const next = () => {
    currentSlide.value = (currentSlide.value + 1) % slides.length;
}

const previous = () => {
    currentSlide.value = (currentSlide.value - 1 + slides.length) % slides.length;
}
</script>

<style scoped>
.slider {
    display: flex;
    justify-content: space-between;
    margin-top:109px;

}
.slider-picker button {
    width: 52px;
    height: 52px;
    border-radius: 100px;
    font-size: 36px;
}

.slider-picker button:first-child {
    border: 1px solid black;
}

.slider-picker button:last-child {
    background: linear-gradient(215.04deg, #F8A3A8 14.41%, #F3C6A5 50.2%, #E5E1AB 85.99%);
    border: none;
}

.slider-body {
    max-width: 1041px;
    width: 100%;
    height: 225px;
    overflow: hidden;
}

.body-quote {
    display: grid;
    gap: 24px;
    overflow: hidden;
}

.slider-body h3 {
    font-size: 32px;
    font-style: italic;
    text-transform: uppercase;
    line-height: 45px;
    font-weight: 500;
}

.slider-body span {
    font-size: 20px;
    opacity: 40%;
    text-transform: uppercase;
}

.slider-picker {
    gap: 20px;
    display: flex;
    align-items: end;
    margin-bottom: 41px;
}

.slider-picker button {
    cursor: pointer;
}

.fade-slide-enter-active, .fade-slide-leave-active {
    transition: opacity 0.5s, transform 0.5s;
}

.fade-slide-enter-from {
    opacity: 0;
    transform: translateX(5px);
}

.fade-slide-leave-to {
    opacity: 0;
    transform: translateX(-5px);
}
</style>