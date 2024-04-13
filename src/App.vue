<script>
    import AppHeader from './components/AppHeader.vue';
    import AppHero from './components/AppHero.vue';
    import AppMainCards from './components/AppMainCards.vue';

    export default {
      components: {
        AppHeader,
        AppHero,
        AppMainCards
      }
    }
</script>

<template>
    <AppHeader></AppHeader>
    <AppHero></AppHero>
    <main>
      <AppMainCards></AppMainCards>
    </main>
</template>

<style lang="scss">
    @use './style/generic';
</style>