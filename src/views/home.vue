<script setup>
import cardproduct from '@/components/cardproduct.vue';
</script>

<template>
  <main>
    <div class="mt-20">
    <img src="../assets/img/PREORDERS!.png" alt="" class="w-full bg-cover bg-center">
  </div>
  </main>

  <div class="bg-[#a7d1e2]"> 
    <div class=" py-24 container mx-auto items-center">
	<section class="flex flex-col-reverse sm:justify-between items-center min-[768px]:flex-row-reverse">
		<!-- Banner left contents -->
		<div class="w-full md:w-2/4 text-left">
			<h1 class="font-general-semibold text-lg sm:text-xl  xl:text-2xl text-center md:text-left text-ternary-dark dark:text-primary-light">
				About Me!
			</h1>
			<p class="font-general-medium mt-2 text-lg sm:text-xl  xl:text-2xl text-center md:text-left leading-none text-gray-400">
				Artist From Indonesia
			</p>

            <p class="font-general-medium mt-2 text-justify  leading-1 ">
Lorem ipsum dolor sit amet, consectetur adipisicing elit. Temporibus quidem quos alias! Voluptate fuga quasi eius rerum iure nostrum nisi minus eligendi provident neque optio sequi pariatur possimus, officiis labore?
			</p>
			<div class="pt-8">

		</div>



		</div>
		<!-- Banner right illustration -->
		<div class="w-full md:w-2/4 text-right float-right">
			<img
				src="../assets/img/wony.png"
				alt="Developer"
			/>
		</div>
	</section>
</div>
</div>

  <div class="container mx-auto py-24">
    <cardproduct />
</div>

</template>
