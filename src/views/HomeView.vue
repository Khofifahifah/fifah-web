<script setup>
import Hero from '@/components/Home/Hero.vue';
import About from '@/components/Home/About.vue';
</script>

<script>
export default {
  methods: {
    goto() {
      window.scrollTo(0, 800);
    },
  },
};
</script>

<template>
  <Hero @eventScroll="goto" />
  <About />
</template>
