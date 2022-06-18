<script setup>
</script>

<template>
  <header class="header--containter">
    <p class="header--title">A Catch 'Em All Directory</p>
    <div class="poke--name-container">
      <label class="poke--name-label">Enter Pokemon: 
      <input id="poke--name" class="poke--input" placeholder="Ditto" />
      </label>
      <button id="poke--name" class="poke-submit">Submit</button>

    </div>
  </header>
</template>

<style> 

@import url('http://fonts.cdnfonts.com/css/pokemon-solid');

* {
  --poke-yellow: #ffcb05;
  --poke-blue: #3466af;
}

.header--containter {
  display: flex;
  flex-wrap: nowrap;
  flex-direction: column;
  align-items: center;
  justify-content: space-evenly;
  margin: 10px;
  border: 1px solid lightgray;
  /* Took out background gradient to add image. */
  /* background: radial-gradient(
    circle at top left, 
    #ff8a00, 
    #f54842); */
  background-image: url(C:\Users\Jerry\Documents\GitHub\project--vue-simple-api\src\assets\poke-banner.jpg);
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  border-radius: 10px 10px 15px 15px;
}

.header--title {
  font-size: 3em;
  font-family: 'Pokemon Solid', sans-serif;
  color: var(--poke-yellow);
  -webkit-text-stroke-width: 2px;
-webkit-text-stroke-color: var(--poke-blue);
}

.poke--name-label {
  font-family: 'Pokemon Solid', sans-serif;
  font-size: 1.25em;
  color: var(--poke-blue);
  -webkit-text-stroke-width: .5px;
-webkit-text-stroke-color: black;
}

.poke--input {
  border-radius: 5px;
}

button {
  background-color: var(--poke-blue);
  border: none;
  color: white;
  padding: 3px;
  text-decoration: none;
  margin: 2px;
  cursor: pointer;
}
</style>
