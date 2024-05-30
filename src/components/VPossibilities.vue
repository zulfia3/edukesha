<script setup>
import Swiper from "swiper";
import { onMounted } from "vue";
import { Pagination} from "swiper/modules";

onMounted(() => {
  const swiper = new Swiper(".swiper", {
    modules: [Pagination],
    spaceBetween: 30,
    loop: "true",
    pagination: {
      el: ".swiper-pagination",
      clickable: true,
    },
  });
});

</script>

<template>
  <section class="possibilities">
    <div class="container">
      <h2>Возможности</h2>
      <div class="row">
        <div class="col-md-6 col-lg-3">
          <div class="possibilities__item">
            <div class="possibilities__item-blue">
              <div class="possibilities__item-img">
                <img src="/mess.png" alt="" />
              </div>
              <div class="possibilities__item-text">Общение с классом</div>
              <p>Видеосвязь</p>
              <p>Чат с классом</p>
            </div>
          </div>
        </div>
        <div class="col-md-6 col-lg-3">
          <div class="possibilities__item">
            <div class="possibilities__item-orange">
              <div class="possibilities__item-img">
                <img src="/comp.png" alt="" />
              </div>
              <div class="possibilities__item-text">Проведение занятий</div>
              <p>Презентация файлов</p>
              <p>Демонстрация экрана</p>
            </div>
          </div>
        </div>
        <div class="col-md-6 col-lg-3">
          <div class="possibilities__item">
            <div class="possibilities__item-blue">
              <div class="possibilities__item-img">
                <img src="/traffic.png" alt="" />
              </div>
              <div class="possibilities__item-text">Посещаемость</div>
              <p>Автоматическое</p>
              <p>отслеживание</p>
              <p>присутствующих</p>
            </div>
          </div>
        </div>
        <div class="col-md-6 col-lg-3">
          <div class="possibilities__item">
            <div class="possibilities__item-orange">
              <div class="possibilities__item-img">
                <img src="/time.png" alt="" />
              </div>
              <div class="possibilities__item-text">История занятий</div>
              <p>Материалы урока</p>
            </div>
          </div>
        </div>
      </div>
      <div class="swiper">
        <div class="swiper-wrapper">
          <div class="swiper-slide col-lg-3">
            <div class="possibilities__item">
              <div class="possibilities__item-blue">
                <div class="possibilities__item-img">
                  <img src="/mess.png" alt="" />
                </div>
                <div class="possibilities__item-text">Общение с классом</div>
                <p>Видеосвязь</p>
                <p>Чат с классом</p>
              </div>
            </div>
          </div>
          <div class="swiper-slide col-lg-3">
            <div class="possibilities__item">
              <div class="possibilities__item-orange">
              <div class="possibilities__item-img">
                <img src="/comp.png" alt="" />
              </div>
              <div class="possibilities__item-text">Проведение занятий</div>
              <p>Презентация файлов</p>
              <p>Демонстрация экрана</p>
            </div>
            </div>
          </div>
          <div class="swiper-slide col-lg-3">
            <div class="possibilities__item">
              <div class="possibilities__item-blue">
                <div class="possibilities__item-img">
                  <img src="/traffic.png" alt="" />
                </div>
                <div class="possibilities__item-text">Посещаемость</div>
                <p>Автоматическое</p>
                <p>отслеживание</p>
                <p>присутствующих</p>
              </div>
            </div>
          </div>
          <div class="swiper-slide col-lg-3">
            <div class="possibilities__item">
              <div class="possibilities__item-orange">
                <div class="possibilities__item-img">
                  <img src="/time.png" alt="" />
                </div>
                <div class="possibilities__item-text">История занятий</div>
                <p>Материалы урока</p>
              </div>
            </div>
          </div>
        </div>
        <div class="swiper-pagination"></div>
      </div>
    </div>
  </section>
</template>

<style scoped>
</style>