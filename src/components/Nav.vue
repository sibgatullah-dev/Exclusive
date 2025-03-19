<template>
    <header class="bg-[#000] py-3">
        <div class="container">
            <div class="flex">
                <div class="left w-[70%] text-right ">
                    <span class="text-[#FAFAFA] text-[14px] leading-[21px] font-normal Poppins">Summer Sale For All Swim Suits And Free Express Delivery - OFF 50%!</span>
                    <a class="text-[#FAFAFA] text-[14px] leading-[21px] font-semibold Poppins ml-2 underline" href="">ShopNow</a>
                </div>
                <div class="right w-[30%] text-right">
                    <select class="text-[#FAFAFA] text-[14px] leading-[21px] font-semibold Poppins bg-black text-right" name="" id="">
                        <option value="">English</option>
                        <option value="">Russian</option>
                        <option value="">Franch</option>
                    </select>
                </div>

            </div>
    
        </div>
    </header>

    <nav class="pt-10">
    <div class="container">
        <div class="flex items-center">
            <div class="w-[20%]">
                <img :src="logo" alt=""> <!--the sign (:) binds the src with the imported logo-->
            </div>
            <div class="w-[40%] ">
                <ul class="flex space-x-12 text-[16px] leading-[24px] font-normal Poppins">
                    <li><a href="">Home</a></li>
                    <li><a href="">Contact</a></li>
                    <li><a href="">About</a></li>
                    <li><a href="">Signup</a></li>
                </ul>
            </div>

            <div class="w-[25%] bg-[#F5F5F5] rounded-[4px] flex  pl-5 pr-3 py-[10px]">
                <div class="w-[70%]">
                    <input class="outline-none " type="text" placeholder="What are you looking for?">
                </div>

                <div class="w-[30%]  position-center relative">
                    <i class="fa-solid  fa-magnifying-glass text-[20px] absolute right-[-4px] top-[50%] translate-[-50%]"></i>
                </div>
            </div>

            <div class="w-[15%]">
                <div class="flex justify-end gap-[24px]">
                    <a href="" class="text-[30px] text-black"><i class="fa-regular fa-heart"></i></a>
                    <a href="" class="text-[30px] text-black"><i class="fa-solid fa-cart-shopping"></i></a>
                    <a href="" class="text-[30px] text-black"><i class="fa-regular fa-user"></i></a>
                </div>
            </div>
        </div>
    </div>
    </nav>
</template>

<script setup>
    import logo from '@/assets/images/logo.png'

</script>