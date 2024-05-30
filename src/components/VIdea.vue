<script setup>
const idea = [
  {
    img: {
      src: "/schadule.png",
      alt: "Составьте расписание<",
    },
    title: "Составьте расписание",
    description:"Выберите время, предмет и класс. Ученики получат уведомление о предстоящем уроке.",
  },
  {
    img: {
      src: "/material.png",
      alt: "Подготовьте материал",
    },
    title: "Подготовьте материал",
    description: "Загружайте необходимые материалы к уроку.",
  },
  {
    img: {
      src: "/tutor.png",
      alt: "Начните урок с учениками",
    },
    title: "Начните урок с учениками",
    description:
      "Задавайте вопросы и вызывайте «к доске» детей с поднятой рукой.",
  },
];
</script>

<template>
  <section class="idea">
    <div class="container">
      <h2>Как это работает?</h2>
      <div class="row">
        <div
          class="col-md-6 col-lg-4"
          v-for="(item, index) in idea"
          :key="index"
        >
          <div class="idea__card">
            <img :src="item.img.src" :alt="item.img.alt" />
            <div class="idea__card-name">{{ item.title }}</div>
            <p>
              {{ item.description }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
</style>