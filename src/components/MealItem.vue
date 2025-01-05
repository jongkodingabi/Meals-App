<template>
  <div
    class="bg-white shadow-md rounded-xl hover:scale-105 transition-all mx-auto"
  >
    <router-link :to="{ name: 'mealDetails', params: { id: meal.idMeal } }">
      <img
        :src="meal.strMealThumb"
        :alt="meal.strMeal"
        class="rounded-t-2xl w-full h-48 object-cover"
      />
    </router-link>
    <div class="p-3">
      <h3 class="font-bold">{{ meal.strMeal }}</h3>
      <p class="mb-4">
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sequi itaque
        reiciendis iste delectus ex pariatur quod ullam veritatis eius tenetur.
      </p>
      <div class="flex items-center justify-start space-x-2">
        <YoutubeButton :href="meal.strYoutube"> YouTube </YoutubeButton>
        <router-link
          :to="{ name: 'mealDetails', params: { id: meal.idMeal } }"
          class="px-3 py-2 rounded border-2 text-white border-emerald-600 bg-emerald-500 hover:bg-emerald-600 transition-colors"
        >
          View
        </router-link>
      </div>
    </div>
  </div>
</template>

<script setup>
import YoutubeButton from "./YoutubeButton.vue";
const { meal } = defineProps({
  meal: {
    required: true,
    type: Object,
  },
});
</script>
