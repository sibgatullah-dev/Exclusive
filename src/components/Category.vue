<template>
    <section class="pt-[80px] ">
        <div class="container pb-[130px] border-b-1 border-[rgba(0,0,0,0.3)]">
            <div class="flex items-center mr-2 mb-6" bis_skin_checked="1">
                <div class="bg-red-500 w-4 h-8 mr-4 rounded" bis_skin_checked="1"></div>
                <span class="text-red-500 font-semibold">Categories</span>
            </div>
            
            <div class="w-full pb-[60px]">
                <h3 class="font-Poppins text-[36px] font-[600] leading-[48px]">Browse By Category</h3>
            </div>
            <div class="flex gap-x-[30px] ">
                <div class="w-1/6" v-for="(category, index) in Category" :key="index">
                    <!-- Category Image and Name -->
                  <a href="">
                    <div class="flex flex-col border-[rgba(0,0,0,0.2)] hover:bg-red-100 hover:border-red-100 border-1 py-[24px] items-center rounded-[4px] justify-center">
                            <img :src="category.image" :alt="category.name" class="w-[42px] h-auto object-contain">
                            <h3 class="text-4 font-Poppins leading-[24px] font-normal pt-4">{{category.name}}</h3>   
                        </div>
                  </a>
                   
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
// Importing images for the products . If this is not done, the images will not be displayed.
import Camera from "@/assets/Category/camera.png";
import Cellphone from "@/assets/Category/CellPhone.png";
import Gamepad from "@/assets/Category/Gamepad.png";
import Headphone from "@/assets/Category/Headphone.png";
import SmartWatch from "@/assets/Category/SmartWatch.png";
import Computer from "@/assets/Category/Computer.png";

const Category = [
    {
        name: "Cellphone",
        image: Cellphone, // Use imported image  
    },
    {
        name: "Computer",
        image: Computer, // Use imported image  
    },
    {
        name: "Gamepad",
        image: Gamepad, // Use imported image  
    },
    {
        name: "Headphone",
        image: Headphone, // Use imported image  
    },
    {
        name: "Camera",
        image: Camera, // Use imported image  
    },
    {
        name: "SmartWatch",
        image: SmartWatch, // Use imported image  
    },

];
</script>