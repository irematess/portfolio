<template>
  <div class="">
    <Header/>
    <article class="bg-white rounded-3xl mt-56 container mx-auto p-24 text-gray">
      <h2 class="text-4xl font-mazius font-bold">hello!</h2>
      <p class="font-avenir text-xl mt-4">I'm Irem, and I am frontend developer.
          Welcome to my portfolio 😎
      </p>
      <div class="mt-8 flex justify-between items-center">
        <div class="text-3xl flex gap-5">
          <a href="https://www.linkedin.com/in/irematees/"><i class="fa-brands fa-linkedin"></i></a>
          <a href="https://github.com/irematess"><i class="fa-brands fa-github"></i></a>                  
          <a href="https://x.com/iremats16"><i class="fa-brands fa-x-twitter"></i></a>                  
          <a href="https://medium.com/@irematees16"><i class="fa-brands fa-medium"></i></a>                  
        </div>
        <div class="flex gap-4 text-base font-bold font-neutral rounded-full ">
            <a href="#" class="btn btn-primary border border-gray rounded-full hover:bg-gray hover:border-white hover:text-white  px-6">VIEW PROJECTS</a>
            <a href="#" class="btn btn-secondary border border-gray rounded-full hover:bg-gray hover:border-white hover:text-white  px-6">GET IN TOCUH</a>
        </div>
        </div>
    </article>
    <About id="about"/>
    <Technologies/>
    <Projects />
    <GetInTouch />
    <Footer/>
  </div>
</template>
<style>
body{
  @apply bg-primary
}
</style>