<template>
    <section class="pt-[120px]">
        <div class="container">
            <div class="w-full pb-7">
                <h3 class="font-Poppins text-[36px] font-[600] leading-[48px]">New Arrivals</h3>
            </div>
            <div class="flex gap-x-[30px]">
                <div class="w-1/4" v-for="(product, index) in products" :key="index">
                    <div class="relative group flex bg-[#F5F5F5] py-[34px] items-center justify-center">
                        <img :src="product.image" :alt="product.name" class="w-[170px] h-auto object-contain">
                        <!-- Add to Cart Button -->
                        <button class="absolute bottom-4 opacity-0 group-hover:opacity-100 transition-opacity bg-black text-white text-sm px-4 py-2 rounded">
                            Add to Cart
                        </button>
                    </div>
                    <div class="short_detail">
                        <h3 class="text-[16px] font-Poppins text-black font-medium leading-6 pb-2 pt-4">{{ product.name }}</h3>
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
        </div>
    </section>
</template>

<script setup>
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
    },
    {
        name: "AK-900 Wired Keyboard",
        image: p2, // Use imported image
        price: "$50",
        originalPrice: "$75",
        rating: 4,
        reviews: 71,
    },
    {
        name: "HAVIT HV-G92 Gamepad",
        image: p1, // Use imported image
        price: "$45",
        originalPrice: "$60",
        rating: 4,
        reviews: 72,
    },
    {
        name: "MSI IPS LCD Gaming Monitor",
        image: p5, // Use imported image
        price: "$250",
        originalPrice: "$300",
        rating: 5,
        reviews: 90,
    },
];
</script>