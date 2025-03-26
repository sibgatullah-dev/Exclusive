<template>
    <section class="pt-[120px] ">
        <div class="container">
            <div class="w-full pb-7">
                <h3 class="font-Poppins text-[36px] font-[600] leading-[48px]">New Arrivals</h3>
            </div>
            <div class="flex gap-x-[30px]">
                <div class="w-1/4">
                    <div class="flex bg-[#F5F5F5] py-[34px] items-center justify-center">
                        <img src="../assets/images/p4.png" alt="">
                    </div>
                    <div class="short_detail">
                        <h3 class="text-[16px] font-Poppins text-black font-medium leading-6 pb-2 pt-4">ASUS FHD Gaming Laptop</h3>
                        <p class="font-Poppins font-medium text-[16px] leading-6"><span class="text-red-400">$700</span><del class="text-[rgba(0,0,0,0.5)] pl-3">$820</del></p>
                    </div>
                    <div class="flex gap-x-3 font-Poppins pt-2">
                        <div class="star space-x-1">
                            <i v-for="star in 5" class="fa-solid fa-star text-[#FFAD33]"></i>
                        </div>
                        <div class="rate">
                            <span class="text-[rgba(0,0,0,0.5)]">(88)</span>
                        </div>
                    </div>
                </div>
                <div class="w-1/4">
                    <div class="flex bg-[#F5F5F5] py-[34px] items-center justify-center">
                        <img src="../assets/images/p2.png" alt="">
                    </div>
                    <div class="short_detail">
                        <h3 class="text-[16px] font-Poppins text-black font-medium leading-6 pb-2 pt-4">AK-900 Wired Keyboard</h3>
                        <p class="font-Poppins font-medium text-[16px] leading-6"><span class="text-red-400">$50</span><del class="text-[rgba(0,0,0,0.5)] pl-3">$75</del></p>
                    </div>
                    <div class="flex gap-x-3 font-Poppins pt-2">
                        <div class="star space-x-1">
                            <i v-for="star in 4" class="fa-solid fa-star text-[#FFAD33]"></i>
                        </div>
                        <div class="rate">
                            <span class="text-[rgba(0,0,0,0.5)]">(71)</span>
                        </div>
                    </div>
                </div>
                <div class="w-1/4">
                    <div class="flex bg-[#F5F5F5] py-[34px] items-center justify-center">
                        <img src="../assets/images/p1.png" alt="">
                    </div>
                    <div class="short_detail">
                        <h3 class="text-[16px] font-Poppins text-black font-medium leading-6 pb-2 pt-4">HAVIT HV-G92 Gamepad</h3>
                        <p class="font-Poppins font-medium text-[16px] leading-6"><span class="text-red-400">$45</span><del class="text-[rgba(0,0,0,0.5)] pl-3">$60</del></p>
                    </div>
                    <div class="flex gap-x-3 font-Poppins pt-2">
                        <div class="star space-x-1">
                            <i v-for="star in 4" class="fa-solid fa-star text-[#FFAD33]"></i>
                        </div>
                        <div class="rate">
                            <span class="text-[rgba(0,0,0,0.5)]">(72)</span>
                        </div>
                    </div>
                </div>
                <div class="w-1/4">
                    <div class="flex bg-[#F5F5F5] py-[34px] items-center justify-center">
                        <img src="../assets/images/p5.png" alt="">
                    </div>
                    <div class="short_detail">
                        <h3 class="text-[16px] font-Poppins text-black font-medium leading-6 pb-2 pt-4">MSI IPS LCD Gaming Monitor</h3>
                        <p class="font-Poppins font-medium text-[16px] leading-6"><span class="text-red-400">$250</span><del class="text-[rgba(0,0,0,0.5)] pl-3">$300</del></p>
                    </div>
                    <div class="flex gap-x-3 font-Poppins pt-2">
                        <div class="star space-x-1">
                            <i v-for="star in 5" class="fa-solid fa-star text-[#FFAD33]"></i>
                        </div>
                        <div class="rate">
                            <span class="text-[rgba(0,0,0,0.5)]">(90)</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>

</script>