<template>
    <div class="elipse"></div>
    <div class="elipse-2"></div>
    <div class="hero-wrapp container">
      <div class="hero-header" :class="{ 'slide-left': isVisible.heroHeader }">
          <div class="hero-title">
              <h1>Built on trust</h1>
          </div>
          <div class="hero-nav">
              <img src="../assets/img/Vector 1.png" alt=""/>
              <ul>
                  <li><a href="">Behance</a></li>
                  <li><a href="">Instagramm</a></li>
                  <li><a href="">Twitter</a></li>
              </ul>
          </div>
      </div>
      <div class="hero-body" :class="{ 'slide-right': isVisible.heroBody }">
          <ButtonComp class="hero-btn">
              Get Started ➜
          </ButtonComp>
          <h1>Driven by <em>innovation</em></h1>
      </div>
      <div class="hero-footer">
          <div class="hero-rewiew">
              <div class="circle-wrapper">
                  <div class="circle"></div>
                  <div class="circle"></div>
                  <div class="circle"></div>
              </div>
              <div class="rewiew-title">
                  <div class="rewiew-star">
                      <img src="../assets/img/Star 1.png" alt=""/>
                      <span>4.9</span>
                  </div>
                  <div class="rewiew-text">
                      <span>2600+ rewiews</span>
                  </div>
              </div>
          </div>
          <div class="hero-about">
              <h4>Lorem ipsum dolor sit amet, consectetur adipiscing elit...</h4>
          </div>
      </div>
    </div>
  </template>
  
  <script setup>
  import { ref, onMounted } from 'vue'
  import ButtonComp from './ui/ButtonComp.vue'
  
  const isVisible = ref({
    heroHeader: false,
    heroBody: false,
    heroFooter: false
  })
  
  onMounted(() => {
    setTimeout(() => {
      isVisible.value.heroHeader = true
      isVisible.value.heroBody = true
      isVisible.value.heroFooter = true
    }, 300); // Задержка для появления анимации
  })
  </script>
  

<style scoped>
.hero-header, .hero-body, .hero-footer {
  opacity: 0;
  transition: opacity 1s ease, transform 1s ease;
}

.hero-header.slide-left {
  opacity: 1;
  transform: translateX(0); /* Конечное положение */
}

.hero-body.slide-right {
  opacity: 1;
  transform: translateX(0); /* Конечное положение */
}

.hero-header, .hero-body {
    transform: translateX(-100%);
}

.hero-body {
    transform: translateX(100%);
}

/* Дополнительные стили для плавности */
.hero-title h1,
.hero-nav ul {
  transition: transform 0.6s ease;
  transform: translateY(20px);
}

.hero-body h1 {
  transition: transform 0.6s ease;
  transform: translateY(20px);
}
</style>
