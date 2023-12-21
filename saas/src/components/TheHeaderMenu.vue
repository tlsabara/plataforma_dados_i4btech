<script setup>
import {ref} from "vue";

const displayMenuItems = ref(true);
const showHeader = ref(true);

</script>

<template>
  <main>
    <nav v-if="showHeader" class="navbar navbar-expand-lg bg-body-tertiary">
      <div class="container">
        <a class="navbar-brand" href="#">Soliddata</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarColor04"
                aria-controls="navbarColor04" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div v-if="displayMenuItems" class="collapse navbar-collapse" id="navbarColor04">
          <ul class="navbar-nav me-auto">
            <li class="nav-item">
              <a class="nav-link active" href="#">Home
                <span class="visually-hidden">(current)</span>
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Financeiro</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Logistica</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Comercial</a>
            </li>
            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" data-bs-toggle="dropdown" href="#" role="button" aria-haspopup="true"
                 aria-expanded="false">Gerenciamento</a>
              <div class="dropdown-menu">
                <a class="dropdown-item" href="#">Usuários</a>
                <a class="dropdown-item" href="#">Integração</a>
                <div class="dropdown-divider"></div>
                <a class="dropdown-item" href="#">Assinatura</a>
                <a class="dropdown-item" href="#">Faturas</a>
              </div>
            </li>
          </ul>
          <ul class="navbar-nav ms-md-auto">
            <li class="nav-item dropdown" data-bs-theme="light">
              <a class="nav-link dropdown-toggle d-flex align-items-center" href="#" id="theme-menu" aria-expanded="false" data-bs-toggle="dropdown" data-bs-display="static" aria-label="Toggle theme">
                <i class="fa-solid fa-circle-half-stroke"></i>
                <span class="d-lg-none ms-2">Toggle theme</span>
              </a>
              <ul class="dropdown-menu dropdown-menu-end">
                <li>
                  <button type="button" class="dropdown-item d-flex align-items-center" data-bs-theme-value="light" aria-pressed="false">
                    <i class="fa fa-sun"></i><span class="ms-2">Light</span>
                  </button>
                </li>
                <li>
                  <button type="button" class="dropdown-item d-flex align-items-center" data-bs-theme-value="dark" aria-pressed="true">
                    <i class="fa fa-moon"></i><span class="ms-2">Dark</span>
                  </button>
                </li>
              </ul>
            </li>
          </ul>
        </div>
        <div v-else class="collapse navbar-collapse" id="navbarColor04">
          <ul class="navbar-nav me-auto">
            <li class="nav-item">
              <a class="nav-link active " href="#">
                <span class="text-opacity-25">Data Analytics Platform</span>
                <span class="small text-info text-opacity-50"> by i4btech</span>
              </a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </main>
</template>

<style scoped>

</style>