<template>
      <div class="font-cookierun-regular container mx-auto pt-24  flex items-center flex-wrap">
  <ul class="flex items-center">
	<li class="inline-flex items-center">
    <router-link to="/" class="text-gray-600">
		<svg class="w-5 h-auto fill-current mx-2 text-gray-400" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="#000000"><path d="M0 0h24v24H0V0z" fill="none"/><path d="M10 19v-5h4v5c0 .55.45 1 1 1h3c.55 0 1-.45 1-1v-7h1.7c.46 0 .68-.57.33-.87L12.67 3.6c-.38-.34-.96-.34-1.34 0l-8.36 7.53c-.34.3-.13.87.33.87H5v7c0 .55.45 1 1 1h3c.55 0 1-.45 1-1z"/></svg>
  </router-link>
	  <svg class="w-5 h-auto fill-current mx-2 text-gray-400" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M0 0h24v24H0V0z" fill="none"/><path d="M10 6L8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6-6-6z"/></svg>
	</li>


	<li class="inline-flex items-center">
	 <router-link to="/catalog"  class="text-gray-600 hover:text-[#84b8d3]">
		Catalog
  </router-link>
	  <svg class="w-5 h-auto fill-current mx-2 text-gray-400" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M0 0h24v24H0V0z" fill="none"/><path d="M10 6L8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6-6-6z"/></svg>
	</li>

	<li class="inline-flex items-center">
	  <a href="#" class="text-gray-600 hover:text-[#84b8d3]">
		Page 3
	  </a>
	</li>
  </ul>
</div>
    <div class="font-cookierun-regular py-24 container mx-auto">

    <div class="flex flex-col justify-between lg:flex-row gap-16 lg:items-center">
      <!-- IMAGES -->
      <div class="flex flex-col gap-6 lg:w-2/4">
        <img src="../assets/img/product/Doggo tote-bag.png" alt="" class="transition-transform duration-500 transform ease-in-out hover:scale-110 w-full w-full h-full aspect-square object-cover rounded-xl" />

      </div>
      <!-- ABOUT -->
      <div class="flex flex-col gap-4 lg:w-2/4">
        <div>
          <span class="text-[#6183ab] font-semibold">Totebag</span>
          <h1 class="text-3xl font-bold">Totebag 30x40 Baby Canvas</h1>
        </div>
        <p class="text-gray-700">
          Behold, The Doggo tote bag! A cute, handheld bag made with soft baby cotton and straight-to-material printing to make sure it doesn’t deteriorate while washing. Each side has a new and redesigned artwork, you can choose one of either those two
        </p>
        <h6 class="text-2xl font-semibold">$ 199.00</h6>
        <div>
    <label for="size" class="block text-sm font-medium text-gray-700">Select Size:</label>
    <select v-model="selectedSize" id="size" name="size" class="mt-1 block w-full p-2 border border-gray-300 rounded-md focus:outline-none focus:ring-indigo-500 focus:border-indigo-500">
      <option value="small">Small</option>
      <option value="medium">Medium</option>
      <option value="large">Large</option>
      <option value="xl">XL</option>
    </select>
    <p class="mt-2 text-sm text-gray-500">Selected Size: {{ selectedSize }}</p>
  </div>
        <div class="flex flex-row items-center gap-12">
          <div class="flex flex-row items-center">
            <button class="bg-gray-200 py-2 px-5 rounded-lg text-[#84b8d3] text-3xl" @click="decrementAmount">-</button>
            <span class="py-4 px-6 rounded-lg">{{ amount }}</span>
            <button class="bg-gray-200 py-2 px-4 rounded-lg text-[#84b8d3] text-3xl" @click="incrementAmount">+</button>
          </div>
          <button class="bg-[#7cb8d2] text-white font-semibold py-3 px-16 rounded-xl h-full">Add to Cart</button>
        </div>
      </div>
    </div>
</div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        images: {
          img1: "../assets/img/product/Doggo tote-bag.png",

        },
        activeImg: "",
        amount: 1
      };
    },
    mounted() {
      // Set initial active image
      this.setActiveImage(this.images.img1);
    },
    methods: {
      setActiveImage(img) {
        this.activeImg = img;
      },
      incrementAmount() {
        this.amount += 1;
      },
      decrementAmount() {
        if (this.amount > 1) {
          this.amount -= 1;
        }
      }
    }
  };
  </script>
  
  <style scoped>
  /* Add your styles here */
  </style>
  