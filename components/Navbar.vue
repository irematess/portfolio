<script setup>
const LINKS = [{path:'#about', title:'about'}, {path:'#project', title:'project'}, {path:'#getintocuh',title:'getintouch'}]
</script>
<template>
    <nav class="flex gap-10 font-neutral max-md:text-sm max-md:gap-1 text-lg items-center max-lg:hidden">
        <a :href="link.path" v-for="(link, index) in LINKS" :key="index"
        class="transition hover:bg-[#2F3634] py-1 px-4 rounded-full ease-in hover:duration-300 duration-300"
        >{{ link.title }}</a>
    </nav>
   
</template>