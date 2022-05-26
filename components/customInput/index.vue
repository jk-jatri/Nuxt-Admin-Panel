<template>
  <div class="relative transition-all ease-in-out" :class="width">
     <input :id="id" :type="text" :placeholder="placeholder" class="customInput peer ">
     <label :for="id" class="customLabel">{{lableName}}</label>
  </div>
</template>

<script>
export default {
     props: ["id", "type", "placeholder", "lableName", "width"]
}
</script>

<style>

</style>