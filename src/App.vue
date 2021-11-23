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
      <!-- Sezione 3 YT -->
      <YouTubeSection></YouTubeSection>
      <!-- Sezione Playlist  -->
      <PlaylistCard></PlaylistCard>
      <!-- Mailing section -->
      <MailingSection></MailingSection>
    </main>
    <footer></footer>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar";
import Hero from "@/components/Hero";
import CardContainer from "@/components/CardContainer";
import YouTubeSection from "@/components/YouTubeSection";
import PlaylistCard from "@/components/PlaylistCard";
import MailingSection from "@/components/MailingSection";
export default {
  name: "App",
  components: {
    Navbar,
    Hero,
    CardContainer,
    YouTubeSection,
    PlaylistCard,
    MailingSection,
  },
};
</script>

<style lang="scss">
@import "@/styles/app";
</style>
