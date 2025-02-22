<template>
    <div class="nav-items" :style="{ color: textColor, borderColor: textColor }">
        <ul>
          <li v-for="item in navItems" :key="item.text">
            <a :href="item.href">{{ item.text }}</a>
          </li>
        </ul>
    </div>
</template>

<script setup>
import { ref, defineProps } from 'vue'
defineProps({
  textColor: {
    type: String,
    default: 'black'
  }
})
const navItems = ref([
    {text: 'Home', href: '#'},
    {text: 'Services', href: '#'},
    {text: 'Features', href: '#'},
    {text: 'Prices', href: '#'}
])
</script>

<style>
.nav-items {
    max-width: 542px;
    width: 100%;
    border: 1px solid;
    border-radius: 100px;
    height: 45px;
    align-items: center;
    display: grid;
    z-index: 1;
  }
  .nav-items ul {
    display: flex;
    justify-content: space-between;
    padding: 0;
    margin: 0;
    text-transform: uppercase;
    padding: 0 36px;
    font-size: 18px;
    font-family: "Montserrat", sans-serif;
    font-weight: 400;
  }
  .nav-items a {
    color: v-bind(textColor);
    transition: all 0.3s;
  }

  .nav-items a:hover {
    opacity: 50%;
  }
</style>