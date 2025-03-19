<template>
    <footer class="bg-black py-[80px]">
        <div class="container">
            <div class="flex">
                <div class="w-[25%]">
                    <img :src="flogo" alt="">
                    <h3 class="text-white text-[20px] Poppins py-6 leading-[28px] font-medium">Subscribe</h3>
                    <h3 class="text-white text-[16px] Poppins  leading-[28px] font-normal">Get 10% off your first order</h3>
                </div>

                <div class="w-[15%] text-wrap">
                    <h3 class="text-white text-[20px] Poppins leading-[28px] pt-0 font-medium">Support</h3>
                    <div class="flex flex-col">
                        <a class="text-white text-[16px] Poppins  leading-[28px] font-normal" href="">111 Bijoy sarani, Dhaka,  DH 1515, Bangladesh.</a>
                        <a class="text-white text-[16px] Poppins  leading-[28px] font-normal" href="">exclusive@gmail.com</a>
                        <a class="text-white text-[16px] Poppins  leading-[28px] font-normal" href="">+88015-88888-9999</a>
                    </div>
                </div>
                <div class="w-[20%]"></div>
                <div class="w-[20%]"></div>
            </div>
        </div>
    </footer>
</template>

<script setup>
import flogo from '@/assets/images/flogo.png'
</script>