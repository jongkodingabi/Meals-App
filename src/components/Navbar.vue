<template>
  <header
    class="bg-white shadow h-16 flex justify-between mx-auto overflow-hidden"
  >
    <!-- <div class="text-2xl font-bold p-4">
      Your<span class="text-emerald-600">Meal.</span>
    </div> -->
    <router-link :to="{ name: 'home' }" class="text-2xl font-bold p-4">
      Your<span class="text-emerald-600">Meal.</span>
    </router-link>
    <div class="flex items-center gap-1">
      <router-link
        :to="{ name: 'byName' }"
        class="inline-flex items-center px-2 h-full transition-colors text-emerald-400 hover:text-white font-semibold hover:bg-emerald-300"
      >
        Search
      </router-link>
      <router-link
        :to="{ name: 'byLetter' }"
        class="inline-flex items-center px-2 h-full transition-colors text-emerald-400 hover:text-white font-semibold hover:bg-emerald-300"
      >
        By Letter
      </router-link>
      <router-link
        :to="{ name: 'ingredients' }"
        class="inline-flex items-center px-2 h-full transition-colors text-emerald-400 hover:text-white font-semibold hover:bg-emerald-300"
      >
        By ingredients
      </router-link>
    </div>
  </header>
</template>
