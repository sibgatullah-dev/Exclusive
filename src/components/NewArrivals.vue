<template>
    <section class="pt-[120px]">
        <div class="container">
            <div class="w-full pb-7">
                <h3 class="font-Poppins text-[36px] font-[600] leading-[48px]">New Arrivals</h3>
            </div>
            <div class="flex gap-x-[30px]">
                <div class="w-1/4" v-for="(product, index) in products" :key="index">

                   <div class="div relative w-[250px] h-[240px] bg-[#F5F5F5] shadow-lg hover:shadow-xl transition-shadow duration-300 ease-in-out">
                    <div class=" group flex  py-[34px] items-center  justify-center">
                        <!-- Product Image -->
                        <img :src="product.image" :alt="product.name" class="w-[170px] h-auto object-contain">
                        <!-- Discount percantage -->
                        <div class="bg-[#DB4444] py-1 px-3 text-[12px] text-white font-Poppins font-normal leading-4 rounded-[4px] absolute top-3 left-3">
                        {{ product.discount }}
                        </div>

                        <!-- Add to Cart Button -->
                        <button class="absolute bottom-0 w-full bg-[rgba(0,0,0,0.8)] text-white text-sm px-4 py-[6px 
                        ] font-Poppins text-[18px] transform translate-y-[-100%] opacity-0 transition-all 
                        duration-500 ease-in-out group-hover:translate-y-0 group-hover:opacity-100 delay-150 mouse-pointer cursor-pointer">Add to Cart</button>
                        
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
            <div class="text-center bg-[#]"></div>
        </div>
    </section>
</template>

<script setup>
// Importing images for the products . If this is not done, the images will not be displayed.
import p1 from "@/assets/images/p1.png";
import p2 from "@/assets/images/p2.png";
import p4 from "@/assets/images/p4.png";
import p5 from "@/assets/images/p5.png";

const products = [
    {
        name: "ASUS FHD Gaming Laptop",
        image: p4, // Use imported image
        price: "$700",
        originalPrice: "$820",
        rating: 5,
        reviews: 88,
        discount:'-10%',
    },
    {
        name: "AK-900 Wired Keyboard",
        image: p2, // Use imported image
        price: "$50",
        originalPrice: "$75",
        rating: 4,
        reviews: 71,
        discount:'-35%',
    },
    {
        name: "HAVIT HV-G92 Gamepad",
        image: p1, // Use imported image
        price: "$45",
        originalPrice: "$60",
        rating: 4,
        reviews: 72, 
        discount:'-45%',
    },
    {
        name: "MSI IPS LCD Gaming Monitor",
        image: p5, // Use imported image
        price: "$250",
        originalPrice: "$300",
        rating: 5,
        reviews: 90,
        discount:'-20%',
    },
];
</script>