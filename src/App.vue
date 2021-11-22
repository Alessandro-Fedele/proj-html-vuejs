<template>
  <div id="app">
    <header>
      <Navbar></Navbar>
    </header>
    <main>
      <!-- Sezione 1 - Hero -->
      <Hero></Hero>
      <!-- Sezione 2 -->
      <CardContainer></CardContainer>
    </main>
    <footer></footer>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar";
import Hero from "@/components/Hero";
import CardContainer from "@/components/CardContainer";
export default {
  name: "App",
  components: { Navbar, Hero, CardContainer },
};
</script>

<style lang="scss">
@import "@/styles/app";
</style>
