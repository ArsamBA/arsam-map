<template>
   <div class="enter-map-button">
      <nuxt-link to="/map">Enter Map</nuxt-link>
   </div>
</template>

<script setup lang="ts">

</script>

<style lang="scss">
@import '@/assets/scss/global.scss';
.enter-map-button{
   width: 100%;
   height: 80vh;
   display: flex;
   flex-direction: row;
   align-items: center;
   justify-content: center;

   a {
      background: $primary;
      padding: 15px 20px;
      border-radius: 8px;
   }
}
</style>