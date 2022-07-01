<template>
  <div id="app">
    <TheHeader></TheHeader>

    <TheMain>
      <MeetAuthor></MeetAuthor>
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
import TheMain from './components/TheMain.vue'
import MeetAuthor from './components/MeetAuthor.vue'
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
    TheMain,
    MeetAuthor,
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
