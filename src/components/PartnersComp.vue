<template>
  <div class="partners-wrapp">
    <div class="partners container" :class="{ 'fade-in': isVisible.partners }" ref="partnersElement">
        <img src="../assets/img/Vector.png" alt="">
    </div>
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue'

const isVisible = ref({
  partners: false
})

const partnersElement = ref(null)

onMounted(() => {
  const observer = new IntersectionObserver(
    ([entry]) => {
      if (entry.isIntersecting) {
        // Если блок стал видимым, активируем анимацию
        isVisible.value.partners = true
        observer.disconnect() // Останавливаем наблюдение после первого срабатывания
      }
    },
    {
      threshold: 0.5 // Срабатывает, когда 50% элемента видимо
    }
  )
  
  if (partnersElement.value) {
    observer.observe(partnersElement.value)
  }
})
</script>
<style scoped>
.partners-wrapp {
    border: 1px #0E0E0E66 solid;
    border-width: 1px 0 1px 0;
    margin-top: 100px;
}

.partners {
  opacity: 0;
  transition: opacity 1s ease-in-out;
}

.partners.fade-in {
    opacity: 1;
}

.partners img {
    width: 100%;
    padding: 33px 1px;
}
</style>