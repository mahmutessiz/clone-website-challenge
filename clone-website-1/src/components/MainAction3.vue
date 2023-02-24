<script>

export default {
    methods: {
        changeSlide(event) {
            event.target.classList.add("border-b-0");
            event.target.classList.remove("bg-gray-300");
            event.target.classList.add("bg-gray-100");
        },
    },
}
</script>

<template>
    <div class="text-left">
        <h2 class="font-bold text-5xl">Intuitive & approachable</h2> <br>
        <h3 class="text-3xl font-semibold">Built for start-ups, not just developers and project managers.</h3> <br>
        <p class="text-lg">From founders to designers, from developers to product managers, from HR to marketing to
            operations and finance, collaborate across your entire company.</p>
    </div>
    <div class=" w-full ">
        <div class="flex justify-evenly gap-1 mt-10">
            <h2 class="py-4 px-9 text-lg rounded-t-2xl w-1/2 bg-gray-100 border-b-0 border-2 border-black"
                @click="changeSlide">Intuitive</h2>

            <h2 class="py-4 px-9 text-lg rounded-t-2xl w-1/2 bg-gray-300 z-10 border-b-2 border-black" @click="changeSlide">
                Approachable</h2>
        </div>
        <div class="border-black border-2 rounded-b-xl -mt-0.5 overflow-hidden">
            <img src="../images/63e3dff33ec7533c37c3a71c_tasks.png" alt="">
        </div>
        <br>
    </div>
</template>