<template>
  <div class="hidden md:block w-[300px] p-5 bg-corporateBlack h-screen divide-y divide-corporateGray">
    <div class="py-3">
      <img src="@/assets/images/logo/logo.png" alt="profile" class="rounded-full w-2/5 shadow-md mx-auto"/>
      <div class="leading-tight">
        <h2 class="uppercase font-bold text-xl text-center mt-3 text-corporateGray">Joyonto Karmakar</h2>
        <h2 class="text-sm text-center mt-3 text-corporateGray">admin@domain.com</h2>
      </div>
    </div>
    <div class="mt-5 space-y-2 overflow-y-auto h-[calc(100vh-285px)] py-2">
      <div class="pr-3">
        <NuxtLink to="/" class="block p-4 text-corporate rounded-xl" :class="$route.path === '/' ? 'bg-corporateLight' : 'hover:bg-corporateLight'">
        Dashboard
      </NuxtLink>
      <dropdowns
        :title="'Dropdown'"
        :description="'Card description will goes here'"
        :dropdownClass="dropdownClass"
        :detailsClass="detailsClass"
        :descriptionClass="descriptionClass"
      />
      <NuxtLink to="/services" class="block p-4 text-corporate rounded-xl" :class="$route.path === '/services' ? 'bg-corporateLight' : 'hover:bg-corporateLight'">
        Services
      </NuxtLink>
      <NuxtLink to="/about" class="block p-4 text-corporate rounded-xl" :class="$route.path === '/about' ? 'bg-corporateLight' : 'hover:bg-corporateLight'">
        About
      </NuxtLink>
      <NuxtLink to="/contact" class="block p-4 text-corporate rounded-xl" :class="$route.path === '/contact' ? 'bg-corporateLight' : 'hover:bg-corporateLight'">
        Contact
      </NuxtLink>
      </div>
    </div>
    <p class="text-corporateGray text-xs text-center py-3">All Rights Reserved &copy; <NuxtLink to="https://joyontokarmakar.netlify.app" target="_blank" class="font-bold">Joyonto Karmakar</NuxtLink></p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      dropdownClass: "text-sm text-corporate",
      detailsClass: "block rounded-xl p-4",
      descriptionClass:"text-sm"
    };
  },
};
</script>

<style></style>
