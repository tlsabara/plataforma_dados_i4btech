<script setup>
import TheHeaderMenu from "@/components/TheHeaderMenu.vue";
import TheMainContainer from "@/components/TheMainContainer.vue";
import TheSideMenu from "@/components/TheSideMenu.vue";
import TheFilterBar from "@/components/TheFilterBar.vue";

</script>

<template>
  <main>
    <TheHeaderMenu>

    </TheHeaderMenu>
    <TheMainContainer>
      <TheFilterBar
        dashboard-title="Relatório Financeiro"
        dashboard-description="Relatórios de contas a pagar"
      />
      <TheSideMenu/>

    </TheMainContainer>
  </main>
</template>
