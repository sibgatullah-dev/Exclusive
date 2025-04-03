<template>
    <section class="pt-[120px]">
        <div class="container border-b-1 border-[rgba(0,0,0,0.3)]">
            <div class="flex items-center mr-2 mb-6" bis_skin_checked="1">
                <div class="bg-red-500 w-4 h-8 mr-4 rounded" bis_skin_checked="1"></div>
                <span class="text-red-500 font-semibold">This Month's</span>
            </div>
            <div class="w-full pb-10 flex justify-between items-center">
                <h3 class="font-Poppins text-[36px] font-[600] leading-[48px]">Top Rated Products</h3>
                <a href="" class="text-center bg-[#DB4444] py-4 px-12 text-white rounded-[4px] font-Poppins text-[16px] leading-6 font-medium">View All</a>
            </div>
            <div class="flex gap-x-[30px]">
                <div class="w-1/4" v-for="(product, index) in products" :key="index">

                   <div class="div relative w-full h-[240px] bg-[#F5F5F5]  duration-300 ease-in-out">
                        <div class=" group flex  pt-[34px] items-center  justify-center">
                            <!-- Product Image -->
                            <img :src="product.image" :alt="product.name" class=" object-contain">

                            <!-- Discount percantage -->
                            <div class="bg-[#DB4444] py-1 px-3 text-[12px] text-white font-Poppins font-normal leading-4 rounded-[4px] absolute top-3 left-3">{{ product.discount }}</div>

                            <!-- Add to Cart Button -->
                            <button class="absolute bottom-0 w-full bg-[rgba(0,0,0,0.8)] text-white text-sm font-Poppins py-2 leading-[24px] text-[16px] transform translate-y-[-100%] opacity-0 transition-all 
                            duration-500 ease-in-out group-hover:translate-y-0 group-hover:opacity-100 delay-60 mouse-pointer cursor-pointer">Add to Cart</button>
                            
                        </div>
                   </div>

                    <div class="short_detail">
                        <a href=""><h3 class="text-[16px] font-Poppins text-black font-medium leading-6 pb-2 pt-4">{{ product.name }}</h3></a>
                        <p class="font-Poppins font-medium text-[16px] leading-6">
                            <span class="text-red-400">{{ product.price }}</span>
                            <del class="text-[rgba(0,0,0,0.5)] pl-3">{{ product.originalPrice }}</del>
                        </p>
                    </div>
                    <div class="flex gap-x-3 font-Poppins pt-2">
                        <div class="star space-x-1">
                            <i v-for="star in product.rating" :key="star" class="fa-solid fa-star text-[#FFAD33]"></i>
                        </div>
                        <div class="rate">
                            <span class="text-[rgba(0,0,0,0.5)]">({{ product.reviews }})</span>
                        </div>
                    </div>
                </div>
            </div>
            <!-- // The "View All Products" button -->
            <div class=" w-full py-[118px] text-center ">
                
            </div>
        </div>
    </section>
</template>

<script setup>
// Importing images for the products . If this is not done, the images will not be displayed.
import t1 from "@/assets/images/t1.png";
import t2 from "@/assets/images/t2.png";
import t3 from "@/assets/images/t3.png";
import t4 from "@/assets/images/t4.png";

const products = [
    {
        name: "ASUS FHD Gaming Laptop",
        image: t1, // Use imported image
        price: "$300",
        originalPrice: "$450",
        rating: 5,
        reviews: 150,
        discount:'-25%',
    },
    {
        name: "AK-900 Wired Keyboard",
        image: t2, // Use imported image
        price: "$50",
        originalPrice: "$65",
        rating: 4,
        reviews: 300,
        discount:'-15%',
    },
    {
        name: "HAVIT HV-G92 Gamepad",
        image: t3, // Use imported image
        price: "$400",
        originalPrice: "$460",
        rating: 4,
        reviews: 410, 
        discount:'-15%',
    },
    {
        name: "MSI IPS LCD Gaming Monitor",
        image: t4, // Use imported image
        price: "$150",
        originalPrice: "$200",
        rating: 5,
        reviews: 380,
        discount:'-20%',
    },
];
</script>