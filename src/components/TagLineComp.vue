<template>
  <div class="tagline-wrapp">
    <div class="tagline-first">
        <h1>Building the Future of Cloud Technology Together</h1>
    </div>
    <div class="tagline-second">
        <h1>Driven by Expertise, Committed to Excellence</h1>
    </div>
    <div class="tagline-third">
        <h1>Empowering Businesses with Cloud Expertise</h1>
    </div>
  </div>
</template>

<script setup>

</script>

<style scoped>
.tagline-wrapp {
    position: relative;
    width: 97vw; /* Чтобы занять всю ширину экрана */
    height: 435px;
    overflow: hidden; /* Прячем всё, что выходит за границы */
    margin: 0 auto;
    margin-top: 175px;
}

.tagline-first,
.tagline-second,
.tagline-third {
    position: absolute;
    white-space: nowrap; /* Запрещаем перенос строк */
    font-size: 72px;
    font-style: italic;
    opacity: 40%;
}

.tagline-first {
    left: -100%; /* Уводим за левый край */
    animation: slideIn 15s linear infinite;
}

.tagline-second {
    left: 50%; /* Центрируем */
    transform: translateX(-50%);
    background: linear-gradient(215.04deg, #F8A3A8 14.41%, #F3C6A5 50.2%, #E5E1AB 85.99%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    top: 30%;
}

.tagline-third {
    right: -100%; /* Уводим за правый край */
    animation: slideInReverse 15s linear infinite;
    top: 60%;
}

/* Анимация появления из-за экрана */
@keyframes slideIn {
    0% { left: -100%; }
    50% { left: 10%; } /* Показываем текст в видимой области */
    100% { left: -100%; } /* Уводим обратно */
}

@keyframes slideInReverse {
    0% { right: -100%; }
    50% { right: 10%; }
    100% { right: -100%; }
}

/* Адаптив */
@media (max-width: 1024px) {
    .tagline-wrapp h1 {
        font-size: 48px;
    }
}

@media (max-width: 768px) {
    .tagline-wrapp h1 {
        font-size: 36px;
    }
}

@media (max-width: 480px) {
    .tagline-wrapp h1 {
        font-size: 24px;
    }
}

</style>