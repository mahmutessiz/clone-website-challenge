<script>
export default {
  methods: {
    changeSlide() {
      const element1 = document.getElementById('1');
      const element2 = document.getElementById('2');
      const element3 = document.getElementById('3');
      const image3 = document.getElementById('image3');
      const image2 = document.getElementById('image2');
      const image1 = document.getElementById('image1');

      image3.classList.add('hidden');
      image3.classList.remove('block');
      image2.classList.add('hidden');
      image2.classList.remove('block');
      image1.classList.add('block');
      image1.classList.remove('hidden');

      element1.classList.remove('deactive');
      element1.classList.add('active');

      element2.classList.add('deactive');
      element3.classList.add('deactive');

    },
    changeSlide2() {
      const element1 = document.getElementById('1');
      const element2 = document.getElementById('2');
      const element3 = document.getElementById('3');
      const image1 = document.getElementById('image1');
      const image3 = document.getElementById('image3');
      const image2 = document.getElementById('image2');

      image1.classList.add('hidden');
      image1.classList.remove('block');
      image2.classList.add('block');
      image2.classList.remove('hidden');
      image3.classList.add('hidden');
      image3.classList.remove('block');

      element2.classList.remove('deactive');
      element2.classList.add('active');


      element1.classList.add('deactive');
      element3.classList.add('deactive');

    },
    changeSlide3() {
      const element1 = document.getElementById('1');
      const element2 = document.getElementById('2');
      const element3 = document.getElementById('3');
      const image1 = document.getElementById('image1');
      const image2 = document.getElementById('image2');
      const image3 = document.getElementById('image3');

      image1.classList.add('hidden');
      image1.classList.remove('block');
      image2.classList.add('hidden');
      image2.classList.remove('block');
      image3.classList.add('block');
      image3.classList.remove('hidden');

      element3.classList.remove('deactive');
      element3.classList.add('active');


      element1.classList.add('deactive');
      element2.classList.add('deactive');

    }
  }
}
</script>

<template>
  <div class="w-full">
    <div class="mt-10 flex justify-evenly gap-1">
      <h2 id="1" class="active transition-all duration-100" @click="changeSlide">
        Tasks
      </h2>
      <h2 id="2" class="deactive transition-all duration-100" @click="changeSlide2">
        Docs
      </h2>
      <h2 id="3" class="deactive transition-all duration-100" @click="changeSlide3">
        Spaces
      </h2>
    </div>
    <div class="-mt-0.5 overflow-hidden rounded-b-xl border-2 border-black">
      <img src="../images/tasks.png" class="block" id="image1" alt="" />
      <img src="../images/docs.png" class="hidden" id="image2" alt="" />
      <img src="../images/spaces.png" class="hidden" id="image3" alt="" />
    </div>
    <br />
  </div>
</template>

<style scoped>
.active {
  @apply w-1/3 rounded-t-2xl border-2 border-b-0 border-black bg-gray-100 py-4 px-9 text-lg cursor-pointer;
}

.deactive {
  @apply z-10 w-1/3 rounded-t-2xl border-b-2 border-0 border-black bg-gray-300 py-4 px-9 text-lg cursor-pointer;
}
</style>