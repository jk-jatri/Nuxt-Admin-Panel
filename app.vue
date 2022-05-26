<template>
  <NuxtLayout :name="$route.path === '/login' ? 'exceptional' : $route.path ==='/sign-up' ? 'exceptional' : 'common'">
    <NuxtPage />
  </NuxtLayout>
</template>
