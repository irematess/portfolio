<script setup>
const PROJECTS = [
    {thumbnail:'1',
     title: '10 Fast Finger App'  ,
     desc: 'An application that you can test your typing speed that I developed using event listeners.',
     tech: ['vue', 'tailwind'],
     code: 'https://github.com/irematess/10fastFingerApp',
     demo: 'https://10fast-finger-app.vercel.app/'
    },
    {thumbnail:'2',
     title: 'E-Commerce App',
     desc: 'I developed the interface of the project using tailwind and Vue.JS. I processed the data using Axios and the json-server package I did the routing with the Vue Router package',
     tech: ['vue', 'tailwind'],
     code: 'https://github.com/irematess/e-commerce-app',
     demo: ''
    },
    {thumbnail:'3',
     title: 'User List App',
     desc: 'I developed the interface of the project using tailwind and Vue.JS. Using Rest Api, i received data from external sources and showed this data to the user. I learned how to use the Axios package and Vue Router. I took an avatar picture according to the username using Avatar Api.',
     tech: ['vue', 'tailwind'],
     code: 'https://github.com/irematess/userListApp',
     demo: 'https://user-list-app-eta.vercel.app/'
    },
    {thumbnail:'4',
     title: 'Movie App',
     desc: 'I developed the interface of the project using Vue.JS Using Rest Api, i received data from external sources and showed this data to the user. I processed the data using Axios. I did the routing with the Vue Router package ',
     tech: ['vue'],
     code: 'https://github.com/irematess/movie-app/tree/main/movie-app',
     demo: 'https://movie-app-xhhv.vercel.app/'
    }
]
</script>
<template>
    <article class="container mx-auto mb-72">
    <h3 class="mt-60 flex justify-center text-white font-mazius text-4xl">projects</h3>
    <p class="mt-6 mb-28 flex text-center justify-center text-xl text-white font-avenir font-thin">Some things I’ve worked (or am working) on</p>
    <div class="flex flex-col gap-36 projects">
        <!-- Project -->
        <div class="box grid grid-cols-2 gap-8 text-white" v-for="(project, index) in PROJECTS" :key="index">  
            <img :src="`/_nuxt/assets/img/${project.thumbnail}.png`">
            <div class="flex flex-col justify-center gap-4">
                <p class="font-mazius text-4xl ">{{project.title}}</p>
                <p class="font-avenir text-xl">{{project.desc}}</p>
                <div class="flex justify-between">
                    <div class="flex gap-4">
                        <img v-for="(t, index) in project.tech" :key="index" :src="`/_nuxt/assets/img/${t}.png`" class="w-6 h-6">
                    </div>
                    <div class="flex gap-6">
                        <a :href=project.code class="bg-[#4F5B58] px-4 py-1 rounded-full">VIEW CODE</a>
                        <a :href=project.demo class="bg-[#4F5B58] px-4 py-1 rounded-full" v-if="project.demo">VIEW DEMO</a>
                    </div>
                                
                </div>
            </div>
                       
        </div>
    </div>
    </article>  
</template>
<style>

.box:nth-child(odd){
    
    grid-auto-flow: dense;
    direction: rtl;
    text-align: left;
}
</style>