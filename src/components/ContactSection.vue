
<script setup>


</script>
<template>
   <section class="w-full h-screen grid grid-flow-row grid-cols-1 md:grid-cols-2" id="contact_section">
    <div class="flex justify-center items-center">
        <div class="w-4/5 md:w-1/2">
            <div class="w-full">
                <h1 class="text-white font-bold text-3xl border-b-4 border-orange-600">Contact Me</h1>
            </div>
            <div class="w-full flex mt-4">
                <div class="w-16 h-16 flex items-center"><i class="fa-solid fa-envelope text-orange-600 text-4xl"></i></div>
                <div class="w-4/6 h-16 flex items-center pl-1">
                    <h1 class="text-white font-bold text-left md:text-2xl">sahadmanu4@gmail.com</h1>
                </div>
            </div>
            <div class="w-full flex mt-4">
                <div class="w-16  h-16 flex items-center">
                    <i class="fa-solid fa-phone text-orange-600 text-4xl"></i>
                </div>
                <div class="w-4/6 h-16 flex items-center pl-1">
                    <h1 class="text-white font-bold text-left md:text-2xl">91+ 9207311198</h1>
                </div>
            </div>
            <div class="w-full flex mt-4">
                <div class="w-16  h-16 flex items-center">
                    <i class="fa-solid fa-location-dot text-orange-600 text-4xl"></i>
                </div>
                <div class="w-4/6 h-16 flex items-center pl-1">
                    <h1 class="text-white font-bold text-left md:text-2xl">Malappuram,Kottakkal</h1>
                </div>
            </div>
            <div class="mt-8 w-full flex mb-3">
                <a href="https://github.com/sahad-cp" class="mr-4 text-white text-4xl"><i class="fa-brands fa-github"></i></a>
                <a href="" class="mr-4 text-white text-4xl"><i class="fa-brands fa-square-facebook"></i></a>
                <a href="https://wa.me/qr/2R66TO2U62F6G1" class="mr-4 text-white text-4xl"><i class="fa-brands fa-square-whatsapp"></i></a>
                <a href="https://www.instagram.com/_s.a.h.a.d_c.p_/" class="mr-4 text-white text-4xl"><i class="fa-brands fa-square-instagram"></i></a>
                <a href="https://www.linkedin.com/in/muhammad-sahad-37a6b6236/" class="mr-4 text-white text-4xl"><i class="fa-brands fa-linkedin"></i></a>
            </div>
        </div>
    </div>
    <div class="flex justify-center items-center">
        <div class="w-5/6 bg-white h-96 rounded-lg">
            <form  class="p-5">
                <label for="" class="font-bold" >Name:</label>
                <input type="text" name="name" id="name" class="w-full border pl-2 h-10 my-3 " required placeholder="your name">
                <label for="" class="font-bold ">Email:</label>
                <input type="email" name="email" id="email" class="w-full border pl-2 h-10 my-3"  required placeholder="abcd@gmail.com">
                <label for="" class="font-bold ">Phone:</label>
                <input type="text" name="massage" id="phone" class="w-full border pl-2 h-10 mt-3"  placeholder="Message">
                <input type="submit" value="send" class="w-full text-white bg-orange-600 mt-7 h-10 rounded-md font-bold" >
            </form>
        </div>
    </div>
    
   </section>
</template>

<style scoped>
#contact_section{
    background-image:linear-gradient(360deg,rgb(0, 0, 0,0.8),rgb(0, 0, 0,0.8)), url('../assets/1ca7b34a8d5308a03ae186dfe72caabce0327fe2-1456x816.webp');
    background-repeat: no-repeat;
    background-size: cover;
}

</style>