<template>
  <div class="pricing-wrapp">
    <div class="pricing-header">
        <h2>
            Value-Driven Cloud Plans for Every Business Size
        </h2>
        <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed deiusmod tempor incididunt ut labore et dolore magna</span>
    </div>
    <div class="pricing-body">
        <PriceCard></PriceCard>
        <PriceCard></PriceCard>
    </div>
  </div>
</template>

<script setup>
import PriceCard from './ui/PriceCard.vue'
</script>

<style scoped>
.pricing-wrapp {
    max-width: 960px;
    width: 100%;
    margin: 0 auto;
    margin-top: 175px;
}

.pricing-header {
    max-width: 872px;
    width: 100%;
    display: grid;
    justify-content: space-between;
    text-align: center;
    gap: 38px;
}

.pricing-header h2 {
    font-size: 48px;
    text-transform: uppercase;
    line-height: 58px;
}

.pricing-header span {
    font-size: 20px;
    opacity: 80%;
}

.pricing-body {
    display: flex;
    justify-content: space-between;
    margin-top: 111px;
}
</style>