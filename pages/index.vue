<template>
  <div class="container">
    <Hero />
    <LargeCardDisplay
      v-for="cardInfo in largeCardInfo"
      :key="cardInfo.key"
      :cardsSection="cardInfo"
    />
  </div>
</template>

<script>
import Hero from '../components/Hero'
import LargeCardDisplay from '../components/LargeCardDisplay'
import { largeCardSections } from '@/assets/data.js'
export default {
  components: {
    Hero,
    LargeCardDisplay,
  },
  data() {
    return {
      largeCardInfo: largeCardSections,
    }
  },
}
</script>

<style></style>
