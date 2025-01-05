<template>
  <header class="bg-white shadow h-16 flex justify-between items-stretch">
    <router-link
      :to="{ name: 'home' }"
      class="inline-flex items-center h-full px-5 text-4xl font-bold text-emerald-400 hover:bg-emerald-50"
    >
      Home
    </router-link>
    <div class="flex items-center gap-1">
      <router-link
        :to="{ name: 'byName' }"
        class="inline-flex items-center px-2 h-full transition-colors text-emerald-400 hover:text-white font-semibold hover:bg-emerald-300"
      >
        Search Meals
      </router-link>
      <router-link
        :to="{ name: 'byLetter' }"
        class="inline-flex items-center px-2 h-full transition-colors text-emerald-400 hover:text-white font-semibold hover:bg-emerald-300"
      >
        Meals By Letter
      </router-link>
      <router-link
        :to="{ name: 'ingredients' }"
        class="inline-flex items-center px-2 h-full transition-colors text-emerald-400 hover:text-white font-semibold hover:bg-emerald-300"
      >
        Meals By ingredients
      </router-link>
    </div>
  </header>
</template>
