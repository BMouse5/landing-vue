<template>
  <div class="price-card">
    <div class="card-wrapp">
        <div class="card-title">
            <h4>Basic Plan</h4>
            <span><strong>$38</strong> /Month</span>
        </div>
        <div class="card-list">
            <ul>
                <li>✔ Lorem Ipsum Dolor Sit</li>
                <li>✔ Lorem Ipsum Dolor Sit</li>
                <li>✔ Lorem Ipsum Dolor Sit</li>
                <li>✔ Lorem Ipsum Dolor Sit</li>
                <li>✔ Lorem Ipsum Dolor Sit</li>
            </ul>
        </div>
        <div class="card-btn">
            <ButtonComp class="btn">Purchase Now <span>🡥</span></ButtonComp>
        </div>
    </div>
  </div>
</template>

<script setup>
import ButtonComp from './ButtonComp.vue'
</script>

<style scoped>
.price-card {
    max-width: 465px;
    width: 100%;
    height: 680px;
    border-radius: 25px;
    box-shadow: 4px 7px 27px 0px #00000012;
    padding: 67px 51px;
    transition:all 0.3s;
    cursor: pointer;
}

.price-card:hover {
    transform: scale(1.02);
}

.card-wrapp {
    max-width: 363px;
    width: 100%;
    display: grid;
    gap: 76px;
}

.card-title {
    max-width: 197px;
    width: 100%;
    height: 113px;
    display: grid;
    gap: 18px;
}

.card-title h4 {
    font-size: 25.85px;
    line-height: 31.54px;
}

.card-title strong {
    font-size: 51px;
    line-height: 63px;
}
.card-title span {
    font-size: 25.85px;
}
.card-list {
    width: 100%;
}

.card-list ul {
    display: grid;
    gap: 20.5px;
}

.card-list li {
    font-size: 23px;
    line-height: 28px;
}

.card-list li:last-child {
    opacity: 50%;
}

.card-btn {
    width: 100%;
}

.btn {
    max-width: 305px;
    width: 100%;
    height: 67px;
}

.btn span {
    margin-left: 20px;
}
</style>