<template>
  <header>
    <div class="container">
      <div>
      <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="100" height="100" ></div>
      <div class="text"> Company Name</div>
    </div>
  </header>
    <div class="wrapper">
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <q-menu separate-close-popup>
            <q-list dense>
               <q-item clickable>
                  <q-item-section>
                    <RouterLink to="/about">About</RouterLink>
                  </q-item-section>
               </q-item>
          </q-list>
         </q-menu>
        <RouterLink to="/about">Packages</RouterLink>
        <RouterLink to="/about">Coporate Services</RouterLink>
        <RouterLink to="/about"></RouterLink>

      </nav>
    </div>
  <RouterView />
</template>

<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>



<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
  
}

nav a.router-link-exact-active {
  color: white;
}

nav a.router-link-exact-active:hover {
 
  color: aliceblue;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
  color: white;
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    padding-top: 100px;
    /*display: flex;
    place-items: flex-start;
    flex-wrap: wrap;*/
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
  .container {
 display: grid;
 align-items: center; 
 grid-template-columns: 1fr 1fr 1fr;
 column-gap: 5px;
}

img {
  max-width: 100%;
  max-height:100%;
}

.text {
  font-size: 20px;
  color: white;
}
}
</style>
