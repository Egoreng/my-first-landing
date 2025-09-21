<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated class="bg-black text-white">
      <q-toolbar>
        <q-toolbar-title>Балакирев Егор</q-toolbar-title>

        <q-btn flat label="Обо мне" to="#about" />
        <q-btn flat label="Навыки" to="#skills" />
        <q-btn flat label="Контакты" to="#contacts" />
        <q-btn flat label="Галерея" to="#gallery" />
      </q-toolbar>
    </q-header>

    <q-page-container>
      <div id="about" class="section">

          <div class="q-pa-md">
    <q-parallax>
      <template v-slot:media>
        <img src="../assets/images/IMG_0434.jpg">
      </template>

      <template v-slot:content="scope">
        <div
          class="absolute column items-center"
          :style="{
            opacity: 1 + (0.4 - scope.percentScrolled) * 0.6,
            top: (scope.percentScrolled * 80) + '%',
            left: 0,
            right: 0
          }"
        >
          
          <div class="text-h3 text-white text-center">Обо мне</div>
          <div class="text-h6 text-grey-3 text-center">Привет! Меня зовут Балакирев Егор Александрович. Я начинающий Vue.js разработчик.</div>
        </div>
      </template>
    </q-parallax>
  </div>
      </div>
<hr>
      <div id="skills" class="section">
  <h1 class="text-center">Навыки</h1>
  <div class="row q-col-gutter-md">
    <div class="col-12 col-sm-6 col-md-4">
      <q-card>
        <q-card-section>
          <div class="text-h6 text-center">Vue.js</div>
          <div class="text-subtitle2 text-center">Изучаю основы</div>
        </q-card-section>
      </q-card>
    </div>
    <div class="col-12 col-sm-6 col-md-4">
      <q-card>
        <q-card-section>
          <div class="text-h6 text-center">HTML/CSS</div>
          <div class="text-subtitle2 text-center">Базовые знания</div>
        </q-card-section>
      </q-card>
    </div>
    <div class="col-12 col-sm-6 col-md-4">
      <q-card>
        <q-card-section>
          <div class="text-h6 text-center">JavaScript</div>
          <div class="text-subtitle2 text-center">Понимаю основы</div>
        </q-card-section>
      </q-card>
    </div>
  </div>
</div>
<hr>
      <div id="contacts" class="section">
        <h1 class="text-white text-center">Контакты</h1>
        <p class="text-white text-center">Связаться со мной можно по электронной почте: balakireviegor@yandex.ru</p>
      </div>
<hr>
      <div id="gallery" class="section bg-black">
  <h1 class="text-white text-center">Галерея</h1>
  <p class="text-white text-center">Пример анимированной галереи с использованием QIntersection.</p>

  <div class="q-pa-md">
    <div class="row justify-center q-gutter-sm">
      <q-intersection
        v-for="index in 10"
        :key="index"
        transition="scale"
        class="example-item"
      >
        <q-card flat bordered class="q-ma-sm bg-gray-9">
          <img src="https://cdn.quasar.dev/img/mountains.jpg">

          <q-card-section>
            <div class="text-h6">Card #{{ index }}</div>
            <div class="text-subtitle2">by John Doe</div>
          </q-card-section>
        </q-card>
      </q-intersection>
    </div>
  </div>
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
  padding: 100px 0px;
  min-height: 50vh;
}

#about {
  background-color: #000000;
}

#skills {
  background-color: #000000;
}

#contacts {
  background-color: #000000;
}

#gallery {
  background-color: #000000;
}

.example-item {
  width: 300px; /* Ширина карточки */
  min-height: 200px; /* Минимальная высота */
  height: 300px;
}

</style>