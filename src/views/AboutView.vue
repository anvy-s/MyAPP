<script setup lang="ts">
import TheWelcome from '../components/TheWelcome.vue'
import PackageDetails from '../components/PackageDetails.vue'
</script>
<template>
  <div class="about">
   <!-- <h1>This is an about page</h1>-->
    <PackageDetails />
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
