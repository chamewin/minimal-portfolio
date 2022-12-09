<script lang="ts">
import Intro from './components/Intro.vue';
import Portfolio from './components/Portfolio.vue';
import Contact from './components/Contact.vue';
import Timeline from './components/Timeline.vue';
import Footer from './components/Footer.vue';

export default {
  components: {
    Intro,
    Portfolio,
    Contact,
    Timeline,
    Footer,
  },
};
</script>

<template>
  <Intro />
  <Portfolio />
  <Timeline />
  <Contact />
</template>
