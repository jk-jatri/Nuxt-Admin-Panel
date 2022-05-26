<template>
  <NuxtLayout :name="$route.path === '/login || /sign-up' ? 'exceptional' : 'common'">
    <NuxtPage />
  </NuxtLayout>
</template>
