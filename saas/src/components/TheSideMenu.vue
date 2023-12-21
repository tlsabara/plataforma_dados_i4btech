<script setup>

</script>

<template>
  <div class="offcanvas offcanvas-start" tabindex="-1" id="offcanvasExample" aria-labelledby="offcanvasExampleLabel">
    <div class="offcanvas-header">
      <h5 class="offcanvas-title" id="offcanvasExampleLabel">Filtros</h5>
      <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
    </div>
    <div class="offcanvas-body">
      <div>
        <small>
          Este é o menu de filtros do relatório, faça sua seleção e clique em aplicar.
        </small>
      </div>
      <div class="mt-3">
        <fieldset class="form-group">
          <legend class="mt-4">Empresa</legend>
          <div class="form-check">
            <input class="form-check-input" type="radio" name="optionsRadios" id="optionsRadios1" value="option1" checked="">
            <label class="form-check-label" for="optionsRadios1">
              Apenas dados da Empresa A
            </label>
          </div>
          <div class="form-check">
            <input class="form-check-input" type="radio" name="optionsRadios" id="optionsRadios2" value="option2">
            <label class="form-check-label" for="optionsRadios2">
              Apenas dados da empresa B
            </label>
          </div>
          <div class="form-check disabled">
            <input class="form-check-input" type="radio" name="optionsRadios" id="optionsRadios3" value="option3" disabled="">
            <label class="form-check-label" for="optionsRadios3">
              Empresa 3 - desabilitada
            </label>
          </div>
        </fieldset>
        <fieldset class="form-group">
          <legend class="mt-4">Centro de Custo</legend>
          <div class="form-check">
            <input class="form-check-input" type="checkbox" value="" id="flexCheckDefault">
            <label class="form-check-label" for="flexCheckDefault">
              0001 - TI
            </label>
          </div>
          <div class="form-check">
            <input class="form-check-input" type="checkbox" value="" id="flexCheckChecked" checked="">
            <label class="form-check-label" for="flexCheckChecked">
              0002 - RH
            </label>
          </div>
          <div class="form-check">
            <input class="form-check-input" type="checkbox" value="" id="flexCheckChecked" checked="">
            <label class="form-check-label" for="flexCheckChecked">
              0003 - Data Analytics
            </label>
          </div>
        </fieldset>
        <fieldset class="form-group">
          <legend class="mt-4">Opções extras</legend>
          <div class="form-check form-switch">
            <input class="form-check-input" type="checkbox" id="flexSwitchCheckDefault">
            <label class="form-check-label" for="flexSwitchCheckDefault">Agrupar subdivisões de cento de custo</label>
          </div>
          <div class="form-check form-switch">
            <input class="form-check-input" type="checkbox" id="flexSwitchCheckChecked" checked="">
            <label class="form-check-label" for="flexSwitchCheckChecked">Apenas Contas de fornecedores ativos</label>
          </div>
        </fieldset>
        <fieldset v-if="false" class="form-group">
          <legend class="mt-4">Ranges</legend>
          <label for="customRange1" class="form-label">Example range</label>
          <input type="range" class="form-range" id="customRange1">
          <label for="disabledRange" class="form-label">Disabled range</label>
          <input type="range" class="form-range" id="disabledRange" disabled="">
          <label for="customRange3" class="form-label">Example range</label>
          <input type="range" class="form-range" min="0" max="5" step="0.5" id="customRange3">
        </fieldset>
      </div>
    </div>
  </div>
</template>

<style scoped>

</style>