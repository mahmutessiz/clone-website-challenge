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
        <h2 class="font-bold text-5xl">Unified & integrated</h2> <br>
        <h3 class="text-3xl font-semibold">Everything in the right place.</h3> <br>
        <p class="text-lg">No more searching across different tools, no more paying for two products to do the job of one.
            Superthread provides everything you need and connects with all your other key tools.</p>
    </div>
    <div class=" w-full ">
        <div class="flex justify-evenly gap-1 mt-10">
            <h2 class="py-4 px-9 text-lg rounded-t-2xl w-1/2 bg-gray-100 border-b-0 border-2 border-black"
                @click="changeSlide">Search</h2>

            <h2 class="py-4 px-9 text-lg rounded-t-2xl w-1/2 bg-gray-300 z-10 border-b-2 border-black" @click="changeSlide">
                Integretions</h2>
        </div>
        <div class="border-black border-2 rounded-b-xl -mt-0.5 overflow-hidden">
            <img src="../images/63e3dff33ec7533c37c3a71c_tasks.png" alt="">
        </div>
        <br>
    </div>
</template>