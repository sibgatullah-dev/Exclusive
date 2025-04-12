<template>
 <section class="pt-[120px]">
        <div class="container ">
            <div class="flex items-center mr-2 mb-6" bis_skin_checked="1">
                <div class="bg-red-500 w-4 h-8 mr-4 rounded" bis_skin_checked="1"></div>
                <span class="text-red-500 font-semibold">Our Products</span>
            </div>
            <div class="w-full pb-7">
                <h3 class="font-Poppins text-[36px] font-[600] leading-[48px]">Explore Our Products</h3>
            </div>
            <div class="flex gap-x-[20px] gap-y-[60px] flex-wrap">
                <div class="w-[23.7%]" v-for="(product, index) in products" :key="index"><!--Loop here v-for loop-->

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
                <a href="" class="text-center bg-[#DB4444] py-4 px-12 text-white rounded-[4px] font-Poppins text-[16px] leading-6 font-medium">View All Products</a>
            </div>
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
    {
        name: "MSI IPS LCD Gaming Monitor",
        image: p5, // Use imported image
        price: "$250",
        originalPrice: "$300",
        rating: 5,
        reviews: 90,
        discount:'-20%',
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
    {
        name: "MSI IPS LCD Gaming Monitor",
        image: p5, // Use imported image
        price: "$250",
        originalPrice: "$300",
        rating: 5,
        reviews: 90,
        discount:'-20%',
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


//fake api
// import {onMounted,ref} from 'vue'
// const product = ref([""])
// onMounted(async() => {
//     const response = await fetch('https://dummyjson.com/products')
//     const data = await response.json()
//     const allproducts = data.products
//     product.value = allproducts.map((item) => item)
// })

</script>