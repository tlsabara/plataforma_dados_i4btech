<script setup>
defineProps(
  {
    innerText: String,
    targetId: String
  }
)
</script>

<template>
  <button class="btn btn-primary mx-1" type="button" data-bs-toggle="offcanvas" :data-bs-target="targetId" aria-controls="offcanvasExample">
    {{ innerText }}
  </button>
</template>

<style scoped>

</style>