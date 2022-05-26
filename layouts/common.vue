<template>
  <div class="flex">
    <sidebars />
    <div
      class="w-full md:w-[calc(100%-300px)] h-screen overflow-hidden bg-blue-50"
    >
      <headers />
      <div
        class="m-5 p-4 bg-gray-100 min-h-[calc(100vh-112px)] overflow-auto rounded-md shadow-md"
      >
        <slot />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style></style>
