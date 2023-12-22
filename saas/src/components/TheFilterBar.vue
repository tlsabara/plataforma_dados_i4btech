<script setup>
import ButtonSideMenuControl from "@/components/ButtonSideMenuControl.vue";
defineProps({
  dashboardTitle: String,
  dashboardDescription: String
})
</script>

<template>
  <main>
    <div class="d-flex justify-content-between">
      <div>
        <ButtonSideMenuControl
          inner-text="Filtros"
          target-id="#offcanvasFilter"
        />
        <ButtonSideMenuControl
          inner-text="Exportação"
          target-id="#offcanvasExport"
        />
      </div>
      <div>
        <h4>
          {{ dashboardTitle }}
        </h4>
        <h6>
          {{ dashboardDescription }}
        </h6>
      </div>
    </div>
    <hr>
  </main>
</template>

<style scoped>

</style>