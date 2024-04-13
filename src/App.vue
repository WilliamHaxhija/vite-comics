<script>
    import AppHeader from './components/AppHeader.vue';
    import AppHero from './components/AppHero.vue';
    import AppMainCards from './components/AppMainCards.vue';
    import AppMainFeatures from './components/AppMainFeatures.vue';
    import AppFooter from './components/AppFooter.vue';

    export default {
      components: {
        AppHeader,
        AppHero,
        AppMainCards,
        AppMainFeatures,
        AppFooter
      }
    }
</script>

<template>
    <AppHeader></AppHeader>
    <AppHero></AppHero>
    <main>
      <AppMainCards></AppMainCards>
      <AppMainFeatures></AppMainFeatures>
    </main>
    <AppFooter></AppFooter>
</template>

<style lang="scss">
    @use './style/generic';
</style>