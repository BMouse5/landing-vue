<template>
  <div class="card-wrapp">
    <div class="card-body">
        <div class="card-label" v-if="show">
            <span>Category</span>
        </div>
        <div class="card-text">
            <span>All-in-One Cloud Services</span>
            <img src="../../assets/img/Frame 15.png" alt="">
        </div>
    </div>
  </div>
</template>

<script setup>
import { defineProps } from 'vue';
defineProps ({
    show: {
        type: Boolean,
        default: false
    }
})
</script>

<style scoped>
.card-wrapp {
    max-width: 410px;
    width: 100%;
    height: 331px;
    box-shadow: 4px 7px 27px 0px #00000012;
    padding: 40px 37px;
    border-radius: 15px;
    margin: 0;
    transition: all 0.5s;
    cursor: pointer;
}

.card-wrapp:hover {
    transform: scale(1.02);
    background: rgb(208, 208, 208);
}

.card-body {
    display: grid;
    gap: 157px;
}

.card-label {
    max-width: 143px;
    width: 100%;
    height: 37px;
    border-radius: 100px;
    border: 1px solid #0E0E0E66;
    display: flex;
    align-items: center;
    justify-content: center;
}

.card-label span{
    font-size: 18px;
    font-weight: 500;
    text-transform: uppercase;
}

.card-text {
    display: flex;
    width: 100%;
    justify-content: space-between;
    align-items: center;
    font-size: 24px;
    text-transform: uppercase;
}
</style>