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
  },
}
</script>

<template>
  <div class="w-full py-9 bg-rose-600 grid place-items-center">
    <p class="font-bold">Note:</p> <span>this is just a clone website. This is the orginal website's link: <a
        href="https://www.superthread.com/"
        class="underline text blue font-bold">https://www.superthread.com/</a></span><br>
  </div>

  <main class="text-center">
    <img src="../images/hero-illustration-2.svg" alt="main image" />
    <div class="flex w-full flex-col items-center justify-center gap-9 px-9">
      <h1 class="mt-6 text-6xl font-bold">Tasks & Docs. Together.</h1>
      <p class="text-3xl text-gray-800">
        Unified productivity software for agile start-ups who want to build better products, faster
      </p>
      <button class="w-fit rounded-full bg-black px-4 py-4 font-serif font-bold text-gray-300 transition-all duration-300 hover:border-b-4 hover:border-r-4 hover:border-yellow-500">
        Try for free beta
      </button>
    </div>
    <MainAction />
    <br />
    <img src="../images/divider-1.svg" alt="" />
    <br />
    <MainAction2 />
    <br />
    <div class="w-full py-9 bg-rose-600 grid place-items-center">
      <p class="font-bold">Note:</p> <span>this is just a clone website. This is the orginal website's link: <a
          href="https://www.superthread.com/"
          class="underline text blue font-bold">https://www.superthread.com/</a></span><br>
    </div>
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

  <div class="w-full py-9 bg-rose-600 grid place-items-center">
    <p class="font-bold">Note:</p> <span>This is just a clone website. This is the orginal website's link: <a
      href="https://www.superthread.com/"
      class="underline text blue font-bold">https://www.superthread.com/</a></span><br>
</div></template>
