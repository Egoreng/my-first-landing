
<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated class="bg-primary text-white">
      <q-toolbar>
        <q-toolbar-title>Балакирев Егор</q-toolbar-title>

        <q-btn flat label="Обо мне" to="#about" />
        <q-btn flat label="Навыки" to="#skills" />
        <q-btn flat label="Контакты" to="#contacts" />
      </q-toolbar>
    </q-header>

    <q-page-container>
      <div id="about" class="section">
        <h1>Обо мне</h1>
        <p>Привет! Меня зовут Балакирев Егор Александрович. Я начинающий Vue.js разработчик.</p>
      </div>

      <div id="skills" class="section">
  <h1>Навыки</h1>
  <div class="row q-col-gutter-md">
    <div class="col-12 col-sm-6 col-md-4">
      <q-card>
        <q-card-section>
          <div class="text-h6">Vue.js</div>
          <div class="text-subtitle2">Изучаю основы</div>
        </q-card-section>
      </q-card>
    </div>
    <div class="col-12 col-sm-6 col-md-4">
      <q-card>
        <q-card-section>
          <div class="text-h6">HTML/CSS</div>
          <div class="text-subtitle2">Базовые знания</div>
        </q-card-section>
      </q-card>
    </div>
    <div class="col-12 col-sm-6 col-md-4">
      <q-card>
        <q-card-section>
          <div class="text-h6">JavaScript</div>
          <div class="text-subtitle2">Понимаю основы</div>
        </q-card-section>
      </q-card>
    </div>
  </div>
</div>

      <div id="contacts" class="section">
        <h1>Контакты</h1>
        <p>Связаться со мной можно по электронной почте: balakireviegor@yandex.ru</p>
      </div>
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
  name: 'App',
};
</script>

<style scoped>
.section {
  padding: 60px 20px;
  min-height: 100vh;
}

#about {
  background-color: #f0f8ff;
}

#skills {
  background-color: #e6f7ff;
}

#contacts {
  background-color: #e0f2f1;
}
</style>