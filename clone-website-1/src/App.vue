<script>
import MainNav from './components/MainNav.vue'
import MainSection from './components/MainSection.vue'
export default {
  components: {
    MainNav,
    MainSection,
  },
}
</script>
<template>
  <div class="flex w-full justify-center px-6">
    <div class="max-w-screen-lg">
      <MainNav />
      <MainSection />
    </div>
  </div>
</template>
