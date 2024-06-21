<script setup>
const isHidden = ref(true)
const openMenu = () => {
    console.log('dsfklş')
    console.log(isHidden.value)
    isHidden.value = !isHidden.value
}

</script>
<template>
    <header class="flex max-lg:justify-around justify-between max-md:px-4 px-12 py-6 items-center text-white border-b border-gray text-nowrap">
        <span class="text-5xl italic font-medium font-mazius">irem ateş</span>
        <i class="fa-solid fa-bars lg:hidden text-3xl transition ease-in duration-1000" @click="openMenu"></i>
        
        <nav class="flex gap-16 font-neutral max-md:text-sm max-md:gap-1 text-lg items-center max-lg:hidden">
            <a href="#about" class="transition hover:bg-[#2F3634] hover:py-2 hover:px-4 rounded-full ease-in hover:duration-300 duration-300">ABOUT</a>
            <a href="#project" class="transition hover:bg-[#2F3634] hover:py-2 hover:px-4 rounded-full ease-in hover:duration-300 duration-300">PROJECT</a>
            <a href="#getintouch" class="transition hover:bg-[#2F3634] hover:py-2 hover:px-4 rounded-full ease-in hover:duration-300 duration-300">GET IN TOUCH</a>
        </nav>
    </header>
    <nav class=" w-full bg-white flex flex-col text-center transition ease-in duration-1000 "
    :class="{'hidden':isHidden}"
    >
            <a href="#about" class="transition hover:font-bold hover:py-2 hover:px-4 ease-in hover:duration-300 duration-300">ABOUT</a>
            <a href="#project" class="transition hover:font-bold hover:py-2 hover:px-4  ease-in hover:duration-300 duration-300">PROJECT</a>
            <a href="#getintouch" class="transition hover:font-bold hover:py-2 hover:px-4     ease-in hover:duration-300 duration-300">GET IN TOUCH</a>
        </nav>
</template>