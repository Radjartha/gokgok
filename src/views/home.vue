<script setup>
import cardproduct from '@/components/cardproduct.vue';
</script>

<template>
  <main class="relative">
    <div class="mt-20">
    <img src="../assets/img/PREORDERS!.png" alt="" class="w-full bg-cover bg-center">
  </div>
  <div class="custom-shape-divider-bottom-1707622743">
    <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
        <path d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z" class="shape-fill"></path>
    </svg>
</div>
  </main>

  <section class="bg-[#a0c9fd]"> 
	<div class="pattren-i ">
	<section
		class="container-fluid min-[768px]:mx-24 mx-6 min-[768px]:flex-row flex flex-col-reverse  pb-24 sm:justify-between items-center"
	>
		<!-- Banner left contents -->
		<div class="w-full md:w-1/3 text-left">
			<h1
				class="font-icon text-3xl md:text-3xl xl:text-[55px] text-center min-[768px]:text-left text-[#1b1b1b] uppercase pb-2"
			>
				Wonivero
			</h1>
			<p
				class="font-cookierun-regular mt-2 text-lg sm:text-xl  xl:text-2xl text-center min-[768px]:text-left leading-none text-[#f0f0f0]"
			>
			Heii! I’m Wolfy Vero but most people call me Woni. I take commissions, make comics and occasionally merch when a furry convention pops up. I’m currently a college student majoring in advertising and hoping to make my own furry brand in the future! ^^
			</p>

		</div>

		<!-- Banner right illustration -->
		<div class="w-full md:w-2/3 text-right float-right">
			<img class=""
				src="../assets/img/wony.png"
				alt="Developer"
			/>
		</div>
	</section>
</div>
</section>

	






  <div class="container mx-auto py-24">
	<h1 class="font-cookierun-bold text-lg sm:text-xl  xl:text-2xl text-center md:text-left text-ternary-dark dark:text-primary-light">
				Product!
			</h1>
			<p class="font-cookierun-regular mt-2  text-center md:text-left leading-none ">
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Aperiam adipisci reprehenderit, illo veritatis autem qui assumenda eum labore minima voluptate quidem, optio quia atque, error possimus et impedit molestiae odit!
			</p>
			<div class="mt-8">
    <cardproduct />
</div>
</div>

<div class="container mx-auto"> 
	<section class="rounded-lg bg-[#a0c7d9] px-10 flex sm:justify-between items-center min-[768px]:flex-row">
		<!-- Banner left contents -->
		<div class="w-full md:w-2/4 text-left">
			<h1 class="font-cookierun-bold text-lg sm:text-xl  xl:text-2xl text-left text-ternary-dark dark:text-primary-light">
				More About Me?
			</h1>
			<div class="pt-2">
				<router-link to="/product">
					<button type="button" class="font-cookierun-regular  text-white bg-[#7cb8d2] hover:bg-[#6183ab] focus:ring-4 focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 me-2 mb-2  focus:outline-none ">Detail</button>

			</router-link>	
		</div>

		</div>
		<!-- Banner right illustration -->
		<div class="w-full md:w-1/4 text-right float-right">
			<img
				src="@/assets/img/icon.png"
				alt="Developer"
			/>
		</div>
	</section>
</div>

</template>

<style scoped>
.pattren-i {
	background-image: url('../assets/img/1.png');
	
}


.custom-shape-divider-bottom-1707622743 {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    overflow: hidden;
    line-height: 0;
    transform: rotate(180deg);
}

.custom-shape-divider-bottom-1707622743 svg {
    position: relative;
    display: block;
    width: calc(118% + 1.3px);
    height: 100px;
}

.custom-shape-divider-bottom-1707622743 .shape-fill {
    fill: #a0c9fd;
}

</style>