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
      <!-- Black Plan Cards Section  -->
      <PlanCard></PlanCard>
      <!-- Articles Section -->
      <ArticleCard></ArticleCard>
      <!-- Section Hero 2  -->
      <Hero2></Hero2>
      <!-- Studios-Locations Section  -->
      <StudiosCard></StudiosCard>
      <!-- Banner Video Section -->
      <BannerVideo></BannerVideo>
    </main>
    <footer>
      <Footer></Footer>
    </footer>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar";
import Hero from "@/components/Hero";
import CardContainer from "@/components/CardContainer";
import YouTubeSection from "@/components/YouTubeSection";
import PlaylistCard from "@/components/PlaylistCard";
import MailingSection from "@/components/MailingSection";
import PlanCard from "@/components/PlanCard";
import ArticleCard from "@/components/ArticleCard";
import Hero2 from "@/components/Hero2";
import StudiosCard from "@/components/StudiosCard";
import BannerVideo from "@/components/BannerVideo";
import Footer from "@/components/Footer";
export default {
  name: "App",
  components: {
    Navbar,
    Hero,
    CardContainer,
    YouTubeSection,
    PlaylistCard,
    MailingSection,
    PlanCard,
    ArticleCard,
    Hero2,
    StudiosCard,
    BannerVideo,
    Footer,
  },
};
</script>

<style lang="scss">
@import "@/styles/app";
</style>
