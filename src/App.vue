<template>
  <div class="div">
    <TheHeader/>
    <TheHero />
    <TheAbout />
    <TheAd />
    <TheFooter />
    
  </div>
</template>

<script setup>
import TheHeader from './components/TheHeader.vue';
import TheHero from './components/TheHero.vue';
import TheAbout from './components/TheAbout.vue'
import TheAd from './components/TheAd.vue'
import TheFooter from './components/TheFooter.vue'





</script>





<style lang="scss" scoped>
.div{
  position: relative;
  .side{
    position: absolute;
    top:0;
    right:0;
  }
}
</style>

