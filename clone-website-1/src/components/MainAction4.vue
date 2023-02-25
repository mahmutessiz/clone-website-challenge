<script>
export default {
  methods: {
    changeSlide() {
      const element1 = document.getElementById('41');
      const element2 = document.getElementById('42');

      const image2 = document.getElementById('image42');
      const image1 = document.getElementById('image41');


      image2.classList.add('hidden');
      image2.classList.remove('block');
      image1.classList.add('block');
      image1.classList.remove('hidden');

      element1.classList.remove('deactive');
      element1.classList.add('active');

      element2.classList.add('deactive');
      element2.classList.remove('active');

    },
    changeSlide2() {
      const element1 = document.getElementById('41');
      const element2 = document.getElementById('42');
      const image1 = document.getElementById('image41');
      const image2 = document.getElementById('image42');

      image1.classList.add('hidden');
      image1.classList.remove('block');
      image2.classList.add('block');
      image2.classList.remove('hidden');

      element2.classList.remove('deactive');
      element2.classList.add('active');

      element1.classList.add('deactive');
      element1.classList.remove('active');
    },
  }
}
</script>

<template>
  <div class="text-left">
    <h2 class="text-5xl font-bold">Unified & integrated</h2>
    <br />
    <h3 class="text-3xl font-semibold">Everything in the right place.</h3>
    <br />
    <p class="text-lg">
      No more searching across different tools, no more paying for two products to do the job of
      one. Superthread provides everything you need and connects with all your other key tools.
    </p>
  </div>
  <div class="w-full">
    <div class="mt-10 flex justify-evenly gap-1">
      <h2
        class="w-1/2 rounded-t-2xl border-2 border-b-0 border-black bg-gray-100 py-4 px-9 text-lg"
        id="41"
        @click="changeSlide"
      >
        Search
      </h2>

      <h2
        class="z-10 w-1/2 rounded-t-2xl border-b-2 border-black bg-gray-300 py-4 px-9 text-lg"
        id="42"
        @click="changeSlide2"
      >
        Integretions
      </h2>
    </div>
    <div class="-mt-0.5 overflow-hidden rounded-b-xl border-2 border-black">
      <img src="../images/search.png" class="block" id="image41" alt="">
      <img src="../images/integration.png" class="hidden" id="image42" alt="">
    </div>
    <br />
  </div>
</template>

<style scoped>
.active {
  @apply w-1/2 rounded-t-2xl border-2 border-b-0 border-black bg-gray-100 py-4 px-9 text-lg cursor-pointer;
}

.deactive {
  @apply z-10 w-1/2 rounded-t-2xl border-b-2 border-0 border-black bg-gray-300 py-4 px-9 text-lg cursor-pointer;
}
</style>