<script setup>
</script>

<template>
  <main>
    <nav class="router--nav">
      <ul class="router--links">
        <li><router-link to="/home">Home</router-link></li>
        <li><router-link to="/about">About</router-link></li>
      </ul>
    </nav>

    <section>
        <h2 class="about--project">The reason I created this site.</h2>
        <p class="about--text">
            This project was started to learn more about API's and cement my knowledge of both HTML/CSS.
        </p>
    </section>
    <section>
        <h2 class="att--project">Attribution for art and other things.</h2>
        <p class="attribute--text">
            Favicon: 
            <a href="https://www.flaticon.com/free-icons/pokemon" title="pokemon icons">Pokemon icons created by Darius Dan - Flaticon</a>
        </p>
    </section>
  </main>
</template>

<style>

*::after {
    background-color: lightslategrey;
}
main {
    margin: 0;
    padding: 0;
    display: absolute;
    text-align: center;
    
}

h2 {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    font-size: 18px;
    padding: 5px 0 5px 0;
}

p {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    font-size: 16px;
    padding-top: 5px;
}
.about--project {
    padding: 5px;
}
</style>
