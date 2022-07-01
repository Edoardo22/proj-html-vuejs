<template>
  <div id="app">
    <TheHeader>
      <NavBar></NavBar>
    </TheHeader>

    <TheMain>
      <PubSection></PubSection>
      <PubSection2></PubSection2>
      <ReviewSection></ReviewSection>
      <EventSection></EventSection>
      <NewsSection></NewsSection>
      <AboutSection></AboutSection>
      <ArticlesSection></ArticlesSection>
    </TheMain>

    <TheFooter>

    </TheFooter>

  </div>
</template>

<script>

import TheHeader from './components/TheHeader.vue'
import NavBar from './components/NavBar.vue'
import TheMain from './components/TheMain.vue'
import PubSection from './components/PubSection.vue'
import PubSection2 from './components/PubSection2.vue'
import ReviewSection from './components/ReviewSection.vue'
import EventSection from './components/EventSection.vue'
import NewsSection from './components/NewsSection.vue'
import AboutSection from './components/AboutSection.vue'
import ArticlesSection from './components/ArticlesSection.vue'
import TheFooter from './components/TheFooter.vue'



export default {
  name: 'App',
  components: {
    TheHeader,
    NavBar,
    TheMain,
    PubSection,
    PubSection2,
    ReviewSection,
    EventSection,
    NewsSection,
    AboutSection,
    ArticlesSection,
    TheFooter,
  }
}
</script>

<style lang="scss">
#app {}
</style>
