<script>
export default {
  methods: {
    changeSlide() {
      const element1 = document.getElementById('21');
      const element2 = document.getElementById('22');

      const image2 = document.getElementById('image22');
      const image1 = document.getElementById('image21');


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
      const element1 = document.getElementById('21');
      const element2 = document.getElementById('22');
      const image1 = document.getElementById('image21');
      const image2 = document.getElementById('image22');

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
    <h2 class="text-5xl font-bold">Fast & flexible</h2>
    <br />
    <h3 class="text-3xl font-semibold">No waiting, no frustration, no restrictions.</h3>
    <br />
    <p class="text-lg">
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dolorem quam adipisci alias voluptate ipsum inventore at
      possimus, temporibus culpa tempore rem sequi pariatur debitis laborum corporis, similique voluptatem autem?
      Possimus.
    </p>
  </div>

  <div class="w-full">
    <div class="mt-10 flex justify-evenly gap-1">
      <h2 class="active" id="21" @click="changeSlide">
        Fast
      </h2>

      <h2 class="deactive" id="22" @click="changeSlide2">
        Flexible
      </h2>
    </div>
    <div class="-mt-0.5 overflow-hidden rounded-b-xl border-2 border-black">
      <img src="../images/fast.png" id="image21" class="block" alt="" />
      <img src="../images/flexible.png" id="image22" class="hidden" alt="" />
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
