<template>
    <header class="bg-[#000] py-3">
        <div class="container">
            <div class="flex">
                <div class="left w-[90%] text-center ">
                    <span class="text-[#FAFAFA] text-[14px] leading-[21px] font-normal Poppins">Summer Sale For All Swim Suits And Free Express Delivery - OFF 50%!</span>
                    <a class="text-[#FAFAFA] text-[14px] leading-[21px] font-semibold Poppins ml-2 underline" href="">ShopNow</a>
                </div>
                <div class="right w-[10%]">
                    <select class="text-[#FAFAFA] text-[14px] leading-[21px] font-semibold Poppins bg-black text-right" name="" id="">
                        <option value="">English</option>
                        <option value="">Russian</option>
                        <option value="">Franch</option>
                    </select>
                </div>

            </div>
    
        </div>
    </header>

    <nav>
    <div class="container">
        <div class="flex">
            <div class="w-[20%]">
                <img :src="logo" alt="">                 
            </div>
            <div class="w-[40%]"></div>
            <div class="w-[20%]"></div>
            <div class="w-[20%]"></div>
        </div>
    </div>
    </nav>
</template>

<script setup>
    import logo from '../../public/images/logo.png'

</script>