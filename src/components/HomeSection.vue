
<script setup>

</script>
<template>
    <section class="w-full h-screen grid grid-flow-row grid-cols-1  md:grid-cols-2 " id="homesection" >
        <div class=" flex justify-center items-center">
            <div>
            <h2 class="font-bold text-3xl md:text-6xl text-white">Hi,</h2>
            <h2 class="font-bold text-3xl md:text-6xl text-white">I am <span class="text-orange-600">Sahad</span></h2>
            <h1 class="font-bold text-4xl md:text-7xl text-white">Web Developer</h1>
            <button class="bg-orange-600 text-white py-2 px-3 mt-3"><a href="#contact_section">Contact me</a></button>
            </div>
        </div>
        <div class="flex justify-center items-center">
            <div class="bg-orange-600 w-72 h-72 md:w-80 md:h-80 lg:w-96 lg:h-96 relative overflow-hidden " id="main-img" style="border-radius:63% 37% 71% 29% / 42% 65% 35% 58% ;" >
            </div>
        </div>
    </section>
</template>

<style scoped>
#main-img {
    background-image: url('../assets/IMG-20221024-WA0014.jpg') ;
    background-repeat: no-repeat;
    background-size: cover ;
}
#main-img:hover{
    box-shadow: 0px 0px 10px 1px rgb(255, 255, 255);
}

#homesection{
    background-image: linear-gradient(360deg,rgb(0, 0, 0,0.8),rgb(0, 0, 0,0.8)),url('../assets/top-ide-software.jpeg');
    background-repeat:no-repeat ;
    background-size:cover ;
}
</style>