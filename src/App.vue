<script setup>
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "@/components/HelloWorld.vue";
</script>

<template>
  <div className="header">
    <div>
      <img
          alt="Vue logo"
          class="logo"
          src="@/assets/logo.png"
          height="56"
      />
    </div>
      <nav>
        <RouterLink to="/">Accueil</RouterLink>
        <RouterLink to="/nosjus">Nos Jus</RouterLink>
        <RouterLink to="/lamarque">La Marque</RouterLink>
        <RouterLink to="/notrequalite">Notre Qualité</RouterLink>
        <RouterLink to="/nosengagements">Nos engagements</RouterLink>
      </nav>

  </div>

  <RouterView/>
</template>

<style>
@import "@/assets/base.css";

#app {
  max-width: 1280px;
  margin: 0 auto;

  font-weight: normal;
}

header {
  line-height: 1.5;
  max-height: 100vh;
}

.header {
  padding: 1rem;
  border-bottom: 0.5px solid grey;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

a,
.green {
  text-decoration: none;
  color: black;
  transition: 0.4s;
}

@media (hover: hover) {

}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
}

nav a.router-link-exact-active {
  color: var(--color-text);
  font-weight: bold;
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  /*body {
    display: flex;
    place-items: center;
  }

  #app {
    display: grid;
    grid-template-columns: 1fr 1fr;
    padding: 0 2rem;
  }*/

  .header {
    display: grid;
    grid-template-columns: 1fr 2fr;
    align-items: center;
    justify-items: stretch;
  }

  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  nav {
    font-size: 1rem;
  }
}
</style>
