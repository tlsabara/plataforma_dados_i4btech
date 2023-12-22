<script setup>
defineProps({
  title: String,
  idLabel: String,
  idOffcanvas: String
})
</script>

<template>
  <div class="offcanvas offcanvas-start" tabindex="-1" :id="idOffcanvas" aria-labelledby="offcanvasExampleLabel">
    <div class="offcanvas-header">
      <h3 class="offcanvas-title" :id="idLabel">{{ title }}</h3>
      <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
    </div>
    <div class="offcanvas-body">
      <slot></slot>
    </div>
  </div>
</template>

<style scoped>

</style>