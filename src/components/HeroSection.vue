<template>
  <div class="flex flex-wrap">
    <div class="w-full sm:w-8/12 mb-10">
      <div class="container mx-auto h-full sm:p-10">
        <nav class="flex px-4 justify-between items-center">
          <!-- <div class="text-4xl font-bold">
            Your<span class="text-emerald-600">Meal.</span>
          </div> -->
          <div>
            <img
              src="https://image.flaticon.com/icons/svg/497/497348.svg"
              alt=""
              class="w-8"
            />
          </div>
        </nav>
        <header
          class="container px-4 lg:flex mt-10 items-center h-full lg:mt-0"
        >
          <div class="w-full">
            <h1 class="text-4xl lg:text-6xl font-bold">
              Find your <span class="text-emerald-600"> delicious</span> Meals
            </h1>
            <div class="w-20 h-2 bg-emerald-600 my-4"></div>
            <p class="text-xl mb-10">
              Go on an adventure to find your favorite, delicious,
              <span class="text-emerald-500"
                >and interesting food, and also your way to make your favorite
                food.</span
              >
            </p>
            <MainButton>See More</MainButton>
          </div>
        </header>
      </div>
    </div>
    <img
      src="/img/meals.jpg"
      alt="Food"
      class="w-full h-48 object-cover sm:h-screen sm:w-4/12 rounded-b-full mb-8"
    />
  </div>
</template>

<script setup>
import MainButton from "./MainButton.vue";
</script>
