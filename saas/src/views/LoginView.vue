<script setup>
import TheHeaderMenu from "@/components/TheHeaderMenu.vue";
import TheMainContainer from "@/components/TheMainContainer.vue";

</script>

<template>
  <main>
    <TheHeaderMenu>

    </TheHeaderMenu>

    <TheMainContainer>
      <div class="d-flex justify-content-center">
        <form action="/" style="max-width: 60%">
          <div class="form-group py-3">
            <label class="form-label mt-4">Login</label>
            <div class="form-floating mb-3">
              <input type="email" class="form-control" id="floatingInput" placeholder="name@example.com">
              <label for="floatingInput">Email address</label>
            </div>
            <div class="form-floating mb-3">
              <input type="password" class="form-control" id="floatingPassword" placeholder="Password" autocomplete="off">
              <label for="floatingPassword">Password</label>
            </div>
          </div>
          <div class="py-3 d-flex justify-content-between gap-3" >
            <button class="btn btn-success" type="submit">Login</button>
            <button type="button" class="btn btn-info">Esqueci minha senha</button>
          </div>
        </form>
      </div>
    </TheMainContainer>
  </main>
</template>

<style scoped>
</style>
