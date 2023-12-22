<script setup>

</script>

<template>
  <main>
    <div>
      <small>
        Este é o menu para exportar dados dos relatórios.
      </small>
    </div>
    <hr>
    <div class="d-flex justify-content-between">
      <div class="float-start flex-fill">
        <fieldset class="form-group">
          <legend class="mt-4">Tipo de Exportação</legend>
          <div class="form-check">
            <input class="form-check-input" type="radio" name="optionsRadios" id="optionsRadios1" value="option1" checked="">
            <label class="form-check-label" for="optionsRadios1">
              PDF
            </label>
          </div>
          <div class="form-check">
            <input class="form-check-input" type="radio" name="optionsRadios" id="optionsRadios2" value="option2">
            <label class="form-check-label" for="optionsRadios2">
              Excel
            </label>
          </div>
          <div class="form-check disabled">
            <input class="form-check-input" type="radio" name="optionsRadios" id="optionsRadios3" value="option3" disabled="">
            <label class="form-check-label" for="optionsRadios3">
              CSV
            </label>
          </div>
          <div class="form-check disabled">
            <input class="form-check-input" type="radio" name="optionsRadios" id="optionsRadios3" value="option3" disabled="">
            <label class="form-check-label" for="optionsRadios3">
              Parquet
            </label>
          </div>
          <div class="form-check disabled">
            <input class="form-check-input" type="radio" name="optionsRadios" id="optionsRadios3" value="option3" disabled="">
            <label class="form-check-label" for="optionsRadios3">
              JSON
            </label>
          </div>
          <hr>
          <div class="">
            <button type="button" class="btn btn-info">Exportar</button>
          </div>
        </fieldset>
      </div>
    </div>
  </main>
</template>

<style scoped>

</style>