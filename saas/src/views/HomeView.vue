<script setup>
import TheHeaderMenu from "@/components/TheHeaderMenu.vue";
import TheMainContainer from "@/components/TheMainContainer.vue";
import TheSideMenu from "@/components/TheSideMenu.vue";
import TheFilterBar from "@/components/TheFilterBar.vue";
import FilterSideBody from "@/components/SideBodies/FilterSideBody.vue";
import ExportSideBody from "@/components/SideBodies/ExportSideBody.vue";

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
      <TheSideMenu
        title="Filtros"
        id-label="offcanvasFilterLabel"
        id-offcanvas="offcanvasFilter"
      >
        <FilterSideBody/>
      </TheSideMenu>
      <TheSideMenu
        title="Exportação"
        id-label="offcanvasExportLabel"
        id-offcanvas="offcanvasExport"
      >
        <ExportSideBody/>
      </TheSideMenu>

      <div class="position-absolute top-0 end-0 mt-5 mx-5 p-0 toast show text-dark" role="alert" aria-live="assertive" aria-atomic="true">
        <div class="toast-header">
          <strong class="me-auto text-success">Exportação concluída!</strong>
          <small>Agora</small>
          <button type="button" class="btn-close ms-2 mb-1" data-bs-dismiss="toast" aria-label="Close">
            <span aria-hidden="true"></span>
          </button>
        </div>
        <div class="toast-body">
          Sua exportação foi concluida com sucesso.
        </div>
      </div>


    </TheMainContainer>
  </main>
</template>
