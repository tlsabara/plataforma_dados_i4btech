<script setup>
import TheHeaderMenu from "@/components/TheHeaderMenu.vue";
import TheMainContainer from "@/components/TheMainContainer.vue";
import TheSideMenu from "@/components/TheSideMenu.vue";
import TheFilterBar from "@/components/TheFilterBar.vue";
import FilterSideBody from "@/components/SideBodies/FilterSideBody.vue";
import ExportSideBody from "@/components/SideBodies/ExportSideBody.vue";
import ToastToRemake from "@/components/ToastToRemake.vue";

</script>

<template>
    <main>
        <TheHeaderMenu/>
        <TheMainContainer>
            <TheFilterBar
                    dashboard-title="Home"
                    dashboard-description="Interface de relatórios"
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


            <ToastToRemake
                    variant="success"
            >
                <template v-slot:time>Hoje</template>
                <template v-slot:title>Exportação concluida</template>
                <template v-slot:message>
                    Sua exportação foi concluida com sucesso!!!
                </template>
            </ToastToRemake>

            <div class="row d-flex justify-content-center">
                <div class="col col-6 d-grid gap-2">
                    <button class="btn btn-lg btn-primary" type="button">
                        <h4 class="text-white">Financeiro</h4>
                    </button>
                    <button class="btn btn-lg btn-primary" type="button">
                        <h4 class="text-white">Comercial</h4>
                    </button>
                    <button class="btn btn-lg btn-primary" type="button">
                        <h4 class="text-white">Logistica</h4>
                    </button>
                </div>
            </div>


        </TheMainContainer>
    </main>
</template>
