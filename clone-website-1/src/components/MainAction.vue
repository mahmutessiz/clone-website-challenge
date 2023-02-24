<script>
export default {
  methods: {
    changeSlide(event) {
      event.target.classList.add('border-b-0')
      event.target.classList.remove('bg-gray-300')
      event.target.classList.add('bg-gray-100')
    }
  }
}
</script>

<template>
  <div class="w-full">
    <div class="mt-10 flex justify-evenly gap-1">
      <h2
        class="w-1/3 rounded-t-2xl border-2 border-b-0 border-black bg-gray-100 py-4 px-9 text-lg"
        @click="changeSlide"
      >
        Tasks
      </h2>
      <h2
        class="z-10 w-1/3 rounded-t-2xl border-b-2 border-black bg-gray-300 py-4 px-9 text-lg"
        @click="changeSlide"
      >
        Docs
      </h2>
      <h2
        class="z-10 w-1/3 rounded-t-2xl border-b-2 border-black bg-gray-300 py-4 px-9 text-lg"
        @click="changeSlide"
      >
        Spaces
      </h2>
    </div>
    <div class="-mt-0.5 overflow-hidden rounded-b-xl border-2 border-black">
      <img src="../images/63e3dff33ec7533c37c3a71c_tasks.png" alt="" />
    </div>
    <br />
  </div>
</template>
