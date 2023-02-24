<script>
import MainAction from './MainAction.vue'
import MainAction2 from './MainAction2.vue'
import MainAction3 from './MainAction3.vue'
import MainAction4 from './MainAction4.vue'
import MainBottom from './MainBottom.vue'

export default {
  components: {
    MainAction,
    MainAction2,
    MainAction3,
    MainAction4,
    MainBottom
  }
}
</script>

<template>
  <main class="text-center">
    <img src="../images/hero-illustration-2.svg" alt="main image" />
    <div class="flex w-full flex-col items-center justify-center gap-9 px-9">
      <h1 class="mt-6 text-6xl font-bold">Tasks & Docs. Together.</h1>
      <p class="text-3xl text-gray-800">
        Unified productivity software for agile start-ups who want to build better products, faster
      </p>
      <button class="w-fit rounded-full bg-black px-4 py-4 font-serif font-bold text-gray-300">
        Try for free beta
      </button>
    </div>
    <MainAction />
    <br />
    <img src="../images/divider-1.svg" alt="" />
    <br />
    <MainAction2 />
    <br />
    <img src="../images/divider-3.svg" alt="" />
    <br />
    <MainAction3 />
    <br />
    <img src="../images/divider-2.svg" alt="" />
    <br />
    <MainAction4 />
    <br />
    <img src="../images/divider-3.svg" alt="" /><br /><br />
    <MainBottom />
  </main>
</template>
