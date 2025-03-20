<template>
    <footer class="bg-black py-[80px]">
        <div class="container">
            <div class="flex gap-[87px]">
                <div class="w-[20%]">

                    <img :src="flogo" alt="">
                    <h3 class="text-white text-[20px] Poppins py-6 leading-[28px] font-medium">Subscribe</h3>
                    <h3 class="text-white text-[16px] Poppins  leading-[28px] font-normal">Get 10% off your first order</h3>

                </div>

                <div class="w-[15%] text-wrap">
                    <h3 class="text-white text-[20px] Poppins leading-[28px] pt-0 font-medium">Support</h3>

                    <div class="flex flex-col pt-[24px]">
                        <a class="text-white text-[16px] Poppins  leading-[28px] font-normal" href="">111 Bijoy sarani, Dhaka,  DH 1515, Bangladesh.</a>
                        <a class="text-white text-[16px] Poppins  leading-[28px] font-normal py-4" href="">exclusive@gmail.com</a>
                        <a class="text-white text-[16px] Poppins  leading-[28px] font-normal" href="">+88015-88888-9999</a>
                    </div>

                </div>

                <div class="w-[15%]  ">
                    <h3 class="text-white text-[20px] Poppins leading-[28px] pt-0 font-medium">Account</h3>

                    <div class="flex flex-col pt-[24px]">
                        <a class="text-white text-[16px] Poppins  leading-[28px] font-normal" href="">My Account</a>
                        <a class="text-white text-[16px] Poppins  leading-[28px] font-normal py-4" href="">Login / Register</a>
                        <a class="text-white text-[16px] Poppins  leading-[28px] font-normal" href="">Cart</a>
                        <a class="text-white text-[16px] Poppins  leading-[28px] font-normal pt-4" href="">Wishlist</a>
                    </div>  

                </div>

                <div class="w-[15%]"> 
                    <h3 class="text-white text-[20px] Poppins leading-[28px] pt-0 font-medium">Quick Link</h3>

                    <div class="flex flex-col pt-[24px]">
                        <a class="text-white text-[16px] Poppins  leading-[28px] font-normal" href="">Privacy Policy</a>
                        <a class="text-white text-[16px] Poppins  leading-[28px] font-normal py-4" href="">Terms Of Use</a>
                        <a class="text-white text-[16px] Poppins  leading-[28px] font-normal" href="">FAQ</a>
                        <a class="text-white text-[16px] Poppins  leading-[28px] font-normal pt-4" href="">Contact</a>
                    </div>

                </div> 

                <div class="w-[18%]">
                    <h3 class="text-white text-[20px] Poppins leading-[28px] pt-0 font-medium">Quick Link</h3>

                    <div class="flex py-[24px] items-center">
                        <div class="div">
                            <img :src="Qr_Code" alt="">
                        </div>

                        <div class="div flex flex-col pl-[11px]">
                            <a class="pb-[5px]" href=""><img :src="GooglePlay" alt=""></a>
                            <a href=""><img :src="AppStore" alt=""></a>
                        </div>
                    </div>

                    <div class="flex  gap-6">
                        <a class="text-white text-[24px] font-normal" href=""><i class="fa-brands fa-facebook-f"></i></a>
                        <a class="text-white text-[24px] font-normal" href=""><i class="fa-brands fa-twitter"></i></a>
                        <a class="text-white text-[24px] font-normal" href=""><i class="fa-brands fa-instagram"></i></a>
                        <a class="text-white text-[24px] font-normal" href=""><i class="fa-brands fa-linkedin-in"></i></a>
                    </div>

                </div>
            </div>
        </div>
    </footer>
    <div class="copyright bg-black border-t-[1px] border-[rgba(255,255,255,0.4)] text-[rgba(255,255,255,0.4)] text-[16px] Poppins  leading-[24px] font-normal py-5 text-center">
        <p><span><i class="fa-regular fa-copyright pr-[6px]"></i></span>Copyright Rimel 2022. All right reserved</p>
    </div>
</template>

<script setup>
import flogo from '@/assets/images/flogo.png'
import Qr_Code from '@/assets/images/Qr_Code.png'
import GooglePlay from '@/assets/images/GooglePlay.png'
import AppStore from '@/assets/images/AppStore.png'
</script>