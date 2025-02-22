<template>
  <button class="btn">
    <slot></slot>
  </button>
</template>

<script>
export default {

}
</script>
<style scoped>
.btn {
    padding: 10px;
    max-width: 183px;
    width: 100%;
    height: 50px;
    text-transform: uppercase;
}

</style>