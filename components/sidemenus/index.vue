<template>
  <div class="block md:hidden">
    <div class="w-3/4 h-screen absolute top-0 bottom-0 bg-corporateBlack shadow-lg text-corporate transition-all duration-500 ease-in-out overflow-x-hidden z-10" :class="open ? 'left-0' : '-left-full'">
      <div class="p-5 bg-corporateBlack h-screen divide-y divide-corporateGray">
        <div class="py-2 flex justify-between items-center">
          <img src="@/assets/images/logo/logo.png" alt="profile" class="rounded-full w-[15%] shadow-md"/>
          <div class="text-right">
            <h2 class="uppercase font-bold text-sm text-corporateGray">Joyonto</h2>
            <h2 class="text-sm text-corporateGray">admin@domain.com</h2>
          </div>
        </div>
        <div class="mt-5 space-y-2 overflow-y-auto h-[calc(100vh-150px)] py-2">
          <div class="pr-3">
            <NuxtLink to="/" class="linkClass" :class="$route.path === '/' ? 'linkActiveClass' : 'linkHoverClass'">
              Dashboard
            </NuxtLink>
            <dropdowns
              :title="'Dropdown'"
              :description="'Card description will goes here'"
              :dropdownClass="dropdownClass"
              :detailsClass="detailsClass"
              :descriptionClass="descriptionClass"
            />
            <NuxtLink to="/services" @click="close" class="linkClass" :class="$route.path === '/services' ? 'linkActiveClass' : 'linkHoverClass'">
              Services
            </NuxtLink>
            <NuxtLink to="/about" @click="close" class="linkClass" :class="$route.path === '/about' ? 'linkActiveClass' : 'linkHoverClass'">
              About
            </NuxtLink>
            <NuxtLink to="/contact" @click="close" class="linkClass" :class="$route.path === '/contact' ? 'linkActiveClass' : 'linkHoverClass'">
              Contact
            </NuxtLink>
            <NuxtLink to="/login" @click="close" class="linkClass" :class="$route.path === '/login' ? 'linkActiveClass' : 'linkHoverClass'">
              Login
            </NuxtLink>
            <NuxtLink to="/sign-up" @click="close" class="linkClass" :class="$route.path === '/sign-up' ? 'linkActiveClass' : 'linkHoverClass'">
              Sign Up
            </NuxtLink>
          </div>
        </div>
        <p class="text-corporateGray text-xs text-center py-3">All Rights Reserved &copy; <NuxtLink to="https://joyontokarmakar.netlify.app" target="_blank" class="font-bold">Joyonto Karmakar</NuxtLink></p>
      </div>
    </div>
    <div class="h-screen absolute top-0 bottom-0 bg-black/50 shadow-lg transition-all duration-500 ease-in-out cursor-pointer overflow-x-hidden z-10"
      :class="open ? 'left-3/4 w-1/4' : 'left-full w-0'" @click="close">
    </div>
  </div>
</template>

<script>
export default {
  props: ["open"],
  data() {
    return {
      dropdownClass: "text-sm text-corporateGray",
      detailsClass: "block rounded-xl p-4",
      descriptionClass:"text-sm",
    };
  },
  methods: {
    close() {
      this.$emit("close");
    },
  },
};
</script>

<style></style>
