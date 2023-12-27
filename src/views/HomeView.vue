<script setup lang="ts">
import TheWelcome from '../components/TheWelcome.vue'
import PackageDetails from '../components/PackageDetails.vue'
import Search from '../components/Search.vue'
</script>

<template>
  <main>
    <div><br/></div>
    <Search/>
  </main>
  <div style="display: flex; padding-top: 100px;">
  <PackageDetails />
  </div>
</template>

<style scoped>
.search-box{
  align-items: center;
  font-size: large;
  text-align: center;
}
.button {
  font-size: 18px;
  border-radius: 4px;
  background-color: #a9b502;
  color: white;
  cursor: pointer;
  border: 2px solid #a9b502;;
  height: 50px;
}
</style>