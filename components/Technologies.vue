<script setup>
const TECHNOLOGIES = ['Nuxt','Vue','Javascript','Tailwind', 'Bootstrap','CSS', 'HTML', 'GIT','Github']
</script>
<template>
    <article>
        <div class="flex text-center justify-center text-white font-mazius mt-60 max-lg:mt-20 text-4xl">technologies</div>
        <div class="mt-24 w-3/5 max-lg:w-5/6 mx-auto grid  max-xl:grid-cols-2 grid-cols-3 gap-8 ">
            <div class="rounded-3xl text-center py-24 max-lg:py-8 px-8 bg-gray text-white font-neutral font-semibold" v-for="(tech,index) in TECHNOLOGIES" :key="index"> {{ tech }}</div>
        </div>
    </article>
</template>
