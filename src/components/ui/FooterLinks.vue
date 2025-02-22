<template>
  <div class="links-wrapp">
    <div class="links-body">
        <h4>Our Links</h4>
        <div class="links-href">
            <a href="">Lorem Ipsum</a>   
            <a href="">Lorem Ipsum</a>   
            <a href="">Lorem Ipsum</a>   
            <a href="">Lorem Ipsum</a>   
            <a href="">Lorem Ipsum</a> 
        </div>
    </div>  
  </div>
</template>

<script setup>

</script>

<style scoped>
.links-wrapp {
    max-width: 174px;
    width: 100%;
    color: white;
}
.links-wrapp h4 {
    font-size: 28px;
    font-weight: 400;
}

.links-wrapp a {
    font-size: 20px;
    opacity: 55%;
    color: white;
    font-weight: 400;
}

.links-body {
    display: grid;
    gap: 48px;
}

.links-href {
    display: grid;
    gap: 20px;
}

.links-href a {
    transition: all 0.3s;
}

.links-href a:hover {
    opacity: 80%;
}
</style>