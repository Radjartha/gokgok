<template>
    <div class="py-[200px] container mx-auto">
    <div class="flex flex-col justify-between lg:flex-row gap-16 lg:items-center">
      <!-- IMAGES -->
      <div class="flex flex-col gap-6 lg:w-2/4">
        <img src="../assets/img/product/Doggo tote-bag.png" alt="" class="transition-transform duration-500 transform ease-in-out hover:scale-110 w-full w-full h-full aspect-square object-cover rounded-xl" />

      </div>
      <!-- ABOUT -->
      <div class="flex flex-col gap-4 lg:w-2/4">
        <div>
          <span class="text-violet-600 font-semibold">Totebag</span>
          <h1 class="text-3xl font-bold">Totebag 30x40 Baby Canvas</h1>
        </div>
        <p class="text-gray-700">
       Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio mollitia consequuntur suscipit at. Temporibus eum commodi corporis maxime earum, magni animi, iusto necessitatibus corrupti nam optio quibusdam itaque voluptatibus nemo!
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
            <button class="bg-gray-200 py-2 px-5 rounded-lg text-violet-800 text-3xl" @click="decrementAmount">-</button>
            <span class="py-4 px-6 rounded-lg">{{ amount }}</span>
            <button class="bg-gray-200 py-2 px-4 rounded-lg text-violet-800 text-3xl" @click="incrementAmount">+</button>
          </div>
          <button class="bg-violet-800 text-white font-semibold py-3 px-16 rounded-xl h-full">Add to Cart</button>
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
  