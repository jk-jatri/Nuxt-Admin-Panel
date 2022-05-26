<template>
  <div class="hidden md:block w-[300px] p-5">
    <img
      src="https://images.generated.photos/vyaPXjHlqtBnCOz2zGuPFcbo4u9oGehWdZi9jBe1uhU/rs:fit:256:256/czM6Ly9pY29uczgu/Z3Bob3Rvcy1wcm9k/LnBob3Rvcy92M18w/Njk2NTgxLmpwZw.jpg"
      alt="profile"
      class="rounded-full w-2/5 shadow-md mx-auto"
    />
    <p class="uppercase font-bold text-xl text-center mt-3 text-gray-800">
      Joyonto Karmakar
    </p>
    <div class="mt-5 space-y-2">
      <NuxtLink to="/" class="block p-4 hover:text-white rounded-xl" :class="$route.path === '/' ? 'bg-blue-500 text-white' : 'hover:bg-blue-500'">
        Dashboard
      </NuxtLink>
      <dropdowns
        :title="'Dropdown'"
        :description="'Card description will goes here'"
        :dropdownClass="dropdownClass"
        :detailsClass="detailsClass"
        :descriptionClass="descriptionClass"
      />
      <NuxtLink to="/services" class="block p-4 hover:text-white rounded-xl" :class="$route.path === '/services' ? 'bg-blue-500 text-white' : 'hover:bg-blue-500'">
        Services
      </NuxtLink>
      <NuxtLink to="/about" class="block p-4 hover:text-white rounded-xl" :class="$route.path === '/about' ? 'bg-blue-500 text-white' : 'hover:bg-blue-500'">
        About
      </NuxtLink>
      <NuxtLink to="/contact" class="block p-4 hover:text-white rounded-xl" :class="$route.path === '/contact' ? 'bg-blue-500 text-white' : 'hover:bg-blue-500'">
        Contact
      </NuxtLink>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      dropdownClass: "text-sm",
      detailsClass: "block rounded-xl p-4",
      descriptionClass:"text-sm"
    };
  },
};
</script>

<style></style>
