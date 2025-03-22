<template>
<div class="container">
    <div class="flex">
        <div class="w-[20%] border-r-1 border-[rgba(0,0,0,0.28)] pt-10">
            <ul >
                <li class="pb-4" v-for="category in 9"><a class="text-[16px] text-black font-Poppins font-normal leading-6" href="">Women's Fashion</a></li>
                
            </ul>
        </div>
        <div class="w-[80%]">
            <div className="w-full md:w-3/4 flex flex-row h-auto md:h-96 bg-black relative">
            <div className="flex flex-col justify-center items-start text-white w-full md:w-1/3 pl-4 md:pl-16 py-4 md:py-0">
                <div className="flex items-center mb-2">
                <FontAwesomeIcon
                    icon={faApple}
                    className="text-4xl md:text-6xl mr-2 -mt-1 md:-mt-4 mb-2 md:mb-4"
                />
                <h2 className="text-xs md:text-sm font-light -mt-2 md:-mt-6 ml-1 md:ml-2">
                    iPhone 14 Series
                </h2>
                </div>
                    <p className="mt-2 text-3xl md:text-5xl font-medium">Up to 10%</p>
                    <p className="mt-2 md:mt-4 mb-2 md:mb-4 text-2xl md:text-4xl font-medium">
                    off Voucher
                    </p>
                    <a href="#" className="mt-2 md:mt-4 flex items-center group">
                    <span className="text-white text-sm md:text-md border-b-[1px] border-white group-hover:text-gray-300">
                        Shop Now
                    </span>
                    <FontAwesomeIcon
                        icon={faArrowRight}
                        className="ml-2 text-sm md:text-md text-white group-hover:text-gray-300"
                    />
                    </a>
            </div>
        </div>
    </div>
</div>
</template>

<script setup>

</script>