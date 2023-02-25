<script>
export default {
  methods: {
    changeSlide() {
      const element1 = document.getElementById('31');
      const element2 = document.getElementById('32');

      const image2 = document.getElementById('image32');
      const image1 = document.getElementById('image31');


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
      const element1 = document.getElementById('31');
      const element2 = document.getElementById('32');
      const image1 = document.getElementById('image31');
      const image2 = document.getElementById('image32');

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
    <h2 class="text-5xl font-bold">Intuitive & approachable</h2>
    <br />
    <h3 class="text-3xl font-semibold">
      Built for start-ups, not just developers and project managers.
    </h3>
    <br />
    <p class="text-lg">
      From founders to designers, from developers to product managers, from HR to marketing to
      operations and finance, collaborate across your entire company.
    </p>
  </div>

  <div class="w-full">
    <div class="mt-10 flex justify-evenly gap-1">
      <h2
        class="active"
        id="31"
        @click="changeSlide"
      >
        Intuitive
      </h2>

      <h2
        class="deactive"
        id="32"
        @click="changeSlide2"
      >
        Approachable
      </h2>
    </div>
    <div class="-mt-0.5 overflow-hidden rounded-b-xl border-2 border-black">
      <img src="../images/intuitive.png" class="block" id="image31" alt="" />
      <img src="../images/approachable.png" class="hidden" id="image32" alt="">
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