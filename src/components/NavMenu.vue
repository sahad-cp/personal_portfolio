<script setup>
</script>
<template>
    <div class="w-full h-20 flex justify-center items-center shadow-md">
        <nav class="flex space-x-8">
            <li class="font-bold hover:text-orange-600">
                <a href="">Home</a>
            </li>
            <li class="font-bold hover:text-orange-600">
                <a href="#about">About</a>
            </li>
            <li class="font-bold hover:text-orange-600">
                <a href="">Skill</a>
            </li>
            <li class="font-bold hover:text-orange-600">
                <a href=""> Project</a>
            </li>
            <li class="font-bold hover:text-orange-600">
                <a href="#contact">Contact</a>
            </li>
        </nav>
    </div>
</template>

<style  scoped>
li{
    list-style-type: none;
}

li .active-link{
    border-bottom: 3px solid rgb(255, 106, 0);
}
</style> 