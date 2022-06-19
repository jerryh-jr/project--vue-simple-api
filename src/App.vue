<script setup>
import { RouterView } from 'vue-router'
import SiteHeader from '@/components/SiteHeader.vue'
import SiteFooter from '@/components/SiteFooter.vue'
</script>

<template>

  <SiteHeader />

  <RouterView />

  <main>
  </main>
  <SiteFooter />
</template>
<style> 

.router--links {
  display: flex;
  justify-content: space-evenly;
  list-style: none;
}

</style>
