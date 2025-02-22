<template>
    <div class="main-wrapp">
        <HeaderComp></HeaderComp>
        <HeroComp></HeroComp>
        <PartnersComp></PartnersComp>
        <WhyChoose></WhyChoose>
        <AboutUsComp></AboutUsComp>
        <TagLineComp></TagLineComp>
        <PricingComp></PricingComp>
        <TestimonialComp></TestimonialComp>
        <FooterComp></FooterComp>
    </div>
</template>

<script setup>
import HeaderComp from '@/components/HeaderComp.vue'
import HeroComp from '@/components/HeroComp.vue'
import PartnersComp from '@/components/PartnersComp.vue'
import WhyChoose from '@/components/WhyChoose.vue'
import AboutUsComp from '@/components/AboutUsComp.vue'
import TagLineComp from '@/components/TagLineComp.vue'
import PricingComp from '@/components/PricingComp.vue'
import TestimonialComp from '@/components/TestimonialComp.vue'
import FooterComp from '@/components/FooterComp.vue'
</script>

<style>
.main-wrapp {
    position: relative;
    background-color: #FDFDFD;
}
@media screen and (max-width: 1290px){
    /* Ваши CSS стили для экрана ровно 1920px */
    .main-wrapp{
      
    }
  }
</style>