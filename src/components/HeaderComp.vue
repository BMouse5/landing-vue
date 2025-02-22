<template>
  <header class="header">
    <div class="header-wrapp container">
      <img src="../assets/img/logo.png"/>
      <NavItems>
        <slot></slot>
      </NavItems>
    <ButtonComp>
      Contact Us
    </ButtonComp>
  </div>
  </header>
</template>

<script setup>
import NavItems from './ui/NavItems.vue';
import ButtonComp from './ui/ButtonComp.vue';

</script>
<style scoped>
  header {
    display: flex;
    width: 100%;
    align-items: center;
    justify-content: space-between;
    margin: 0 auto;
    height: 45px;
    margin-top: 46.5px;
  }
  .header-wrapp {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 0 auto;
    padding: 0 1px;
  }
  header img {
    max-width: 150px;
    width: 100%;
    height: 35px;
    cursor: pointer;
  }
</style>