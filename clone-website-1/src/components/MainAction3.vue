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
        class="w-1/2 rounded-t-2xl border-2 border-b-0 border-black bg-gray-100 py-4 px-9 text-lg"
        @click="changeSlide"
      >
        Intuitive
      </h2>

      <h2
        class="z-10 w-1/2 rounded-t-2xl border-b-2 border-black bg-gray-300 py-4 px-9 text-lg"
        @click="changeSlide"
      >
        Approachable
      </h2>
    </div>
    <div class="-mt-0.5 overflow-hidden rounded-b-xl border-2 border-black">
      <img src="../images/63e3dff33ec7533c37c3a71c_tasks.png" alt="" />
    </div>
    <br />
  </div>
</template>
