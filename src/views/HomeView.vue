<script setup>
  import {
    onBeforeMount,
    ref,
    toRaw,
  } from 'vue';

  const ditto = ref({});
  onBeforeMount(async () => {
    const request = await fetch('https://pokeapi.co/api/v2/pokemon/ditto');
    ditto.value = await request.json();
    console.log('Ditto', toRaw(ditto.value));
  });
</script>

<template>
  <main class="main--container">
    <nav class="router--nav">
      <ul class="router--links">
        <li><router-link to="/home">Home</router-link></li>
        <li><router-link to="/about">About</router-link></li>
      </ul>
    </nav>
    
    <h1 class="pokemon--name">{{ ditto.name }}</h1>

    <h2>Abilities</h2>
    <ul>
      <li v-for="(ability, index) in ditto.abilities" :key="index">
        <a :href="ability.ability.url" target="_blank">{{ ability.ability.name }}</a>
      </li>
    </ul>

    <h2>Held Items</h2>
    <ul>
      <li v-for="(item, index) in ditto.held_items" :key="index">
        <a :href="item.item.url" target="_blank">{{ item.item.name }}</a>
      </li>
    </ul>
  </main>
</template>

<style>

* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

.main--container {
  display: grid;
  text-align: center;

}

</style>
