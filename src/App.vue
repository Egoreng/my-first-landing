<template>
  <q-layout view="lHh Lpr lFf">
    <!-- Навигационная шапка -->
    <q-header elevated class="bg-primary text-white">
      <q-toolbar>
        <q-toolbar-title>Балакирев Егор</q-toolbar-title>

        <q-btn flat label="Обо мне" to="#about" />
        <q-btn flat label="Навыки" to="#skills" />
        <q-btn flat label="Контакты" to="#contacts" />
      </q-toolbar>
    </q-header>

    <!-- Контейнер для страниц -->
    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
  name: 'App',
};
</script>

<style scoped>
body {
  font-family: 'Arial', sans-serif;
}

.q-header {
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}
html {
  scroll-behavior: smooth;
}
</style>