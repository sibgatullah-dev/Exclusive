<template>
<div class="container">
    <div class="flex">
        <div class="w-[20%] border-r-1 border-[rgba(0,0,0,0.28)] pt-10">
            <ul >
                <li class="pb-4" v-for="category in 9"><a class="text-[16px] text-black font-Poppins font-normal leading-6" href="">Women's Fashion</a></li>
                
            </ul>
        </div>
        <div class="w-[80%] pt-10 pl-10">
            <div class="  bg-black ">
                <div class="banner_inside flex items-center h-auto pt-[58px] pb-[47px] px-[64px]">
                    <div class="w-[50%] flex flex-col justify-center items-start text-white   pl-4 py-4 ">
                        <div class="flex items-center space-x-2">
                            <img src="../assets/apple-logo.png" alt="" class="w-[40px] h-[49px]">
                            <h2 class="text-xs text-[16px] leading-6 font-poppins">iPhone 14 Series</h2>
                        </div>
                        <p class="mt-2 text-[48px] leading-[60px] font-medium">Up to 10%</p>
                        <p class="mt-2 mb-2  text-[48px] leading-[60px] font-medium"> off Voucher</p>
                        <a href="#" class="mt-2  flex items-center group">
                            <span class="text-white text-sm  border-b-[1px] border-white group-hover:text-gray-300">
                                Shop Now
                            </span>
                        
                        </a>
                    </div>
                    <div class="w-[50%]">
                        <img src="../assets/iphone4.jpeg" alt="">
                    </div>

                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script setup>

</script>