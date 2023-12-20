<script setup>
import TheHeaderMenu from "@/components/TheHeaderMenu.vue";
import TheMainContainer from "@/components/TheMainContainer.vue";

</script>

<template>
  <main>
    <TheHeaderMenu>

    </TheHeaderMenu>
    <TheMainContainer>
      <button class="btn btn-primary" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasExample" aria-controls="offcanvasExample">
        Filtros
      </button>
      <hr>
      <div class="offcanvas offcanvas-start" tabindex="-1" id="offcanvasExample" aria-labelledby="offcanvasExampleLabel">
        <div class="offcanvas-header">
          <h5 class="offcanvas-title" id="offcanvasExampleLabel">Filtros</h5>
          <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
        </div>
        <div class="offcanvas-body">
          <div>
            Some text as placeholder. In real life you can have the elements you have chosen. Like, text, images, lists, etc.
          </div>
          <div class="mt-3">
            <fieldset class="form-group">
              <legend class="mt-4">Radio buttons</legend>
              <div class="form-check">
                <input class="form-check-input" type="radio" name="optionsRadios" id="optionsRadios1" value="option1" checked="">
                <label class="form-check-label" for="optionsRadios1">
                  Option one is this and that—be sure to include why it's great
                </label>
              </div>
              <div class="form-check">
                <input class="form-check-input" type="radio" name="optionsRadios" id="optionsRadios2" value="option2">
                <label class="form-check-label" for="optionsRadios2">
                  Option two can be something else and selecting it will deselect option one
                </label>
              </div>
              <div class="form-check disabled">
                <input class="form-check-input" type="radio" name="optionsRadios" id="optionsRadios3" value="option3" disabled="">
                <label class="form-check-label" for="optionsRadios3">
                  Option three is disabled
                </label>
              </div>
            </fieldset>
            <fieldset class="form-group">
              <legend class="mt-4">Checkboxes</legend>
              <div class="form-check">
                <input class="form-check-input" type="checkbox" value="" id="flexCheckDefault">
                <label class="form-check-label" for="flexCheckDefault">
                  Default checkbox
                </label>
              </div>
              <div class="form-check">
                <input class="form-check-input" type="checkbox" value="" id="flexCheckChecked" checked="">
                <label class="form-check-label" for="flexCheckChecked">
                  Checked checkbox
                </label>
              </div>
            </fieldset>
            <fieldset class="form-group">
              <legend class="mt-4">Switches</legend>
              <div class="form-check form-switch">
                <input class="form-check-input" type="checkbox" id="flexSwitchCheckDefault">
                <label class="form-check-label" for="flexSwitchCheckDefault">Default switch checkbox input</label>
              </div>
              <div class="form-check form-switch">
                <input class="form-check-input" type="checkbox" id="flexSwitchCheckChecked" checked="">
                <label class="form-check-label" for="flexSwitchCheckChecked">Checked switch checkbox input</label>
              </div>
            </fieldset>
            <fieldset class="form-group">
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

    </TheMainContainer>
  </main>
</template>
