<template>
  <section class="home">
    <navigation />
    <main-section />
    <section-partners />
    <section-product-description />
    <section-how-it-works />
    <section-talk-to-milla />
    <section-suitcases-ready />
  </section>
</template>

<script>
import Navigation from '../components/Navigation.vue'
import MainSection from '../components/MainSection'
import SectionPartners from '../components/SectionPartners'
import SectionProductDescription from '../components/SectionProductDescription'
import SectionHowItWorks from '../components/SectionHowItWorks'
import SectionTalkToMilla from '../components/SectionTalkToMilla'
import SectionSuitcasesReady from '../components/SectionSuitcasesReady'

export default {
  name: 'Home',
  components: {
    Navigation,
    MainSection,
    SectionHowItWorks,
    SectionProductDescription,
    SectionTalkToMilla,
    SectionPartners,
    SectionSuitcasesReady
  }
}
</script>

<style>
h,
    SectionPricingtml {
  scroll-behavior: smooth;
}

* {
  @apply font-rubik
}

.container-full-section {
  min-height: calc(100vh - 64px);
  @apply w-full py-4 flex
}

header .title {
  font-size: 32px;
}

header .subtitle {
  font-size: 17px;
  @apply font-normal
}

.card .card-body .title {
  @apply text-lg font-normal
}

.card .card-body .subtitle,
.card .card-body .paragraph {
  @apply text-base
}

@media (min-width: 768px) {
  header .title {
    @apply text-4xl
  }

  header .subtitle {
    @apply text-lg
  }

  .container-full-section {
    @apply pt-16
  }
}
</style>