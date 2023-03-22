<template>
  <div class="carousel" id="customers">
    <div class="carousel__container">
      <VueSlickCarousel v-bind="slickSettings">
        <div>
          <div class="carousel__item">
            <div class="carousel__item__qu">
              <img src="@/assets/img/carousel/qu.svg" alt="" />
            </div>
            <div class="carousel__item__line">
              <img src="@/assets/img/carousel/line.svg" alt="" />
            </div>
            <div class="carousel__item__content">
              <h1>
                Finsweet has been a wonderful partner to work with. I have been
                a customer now for the past few months now and I have had
                nothing but positive experiences!
              </h1>
              <div class="carousel__item__person">
                <img src="@/assets/img/carousel/person.webp" alt="person" />
                <div class="carousel__item__person__text">
                  <h3>Johnny Andro</h3>
                  <p>Director, Company</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div>
          <div class="carousel__item">
            <div class="carousel__item__qu">
              <img src="@/assets/img/carousel/qu.svg" alt="" />
            </div>
            <div class="carousel__item__line">
              <img src="@/assets/img/carousel/line.svg" alt="" />
            </div>
            <div class="carousel__item__content">
              <h1>
                Finsweet has been a wonderful partner to work with. I have been
                a customer now for the past few months now and I have had
                nothing but positive experiences!
              </h1>
              <div class="carousel__item__person">
                <img src="@/assets/img/carousel/person.webp" alt="person" />
                <div class="carousel__item__person__text">
                  <h3>Johnny Andro</h3>
                  <p>Director, Company</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div>
          <div class="carousel__item">
            <div class="carousel__item__qu">
              <img src="@/assets/img/carousel/qu.svg" alt="" />
            </div>
            <div class="carousel__item__line">
              <img src="@/assets/img/carousel/line.svg" alt="" />
            </div>
            <div class="carousel__item__content">
              <h1>
                Finsweet has been a wonderful partner to work with. I have been
                a customer now for the past few months now and I have had
                nothing but positive experiences!
              </h1>
              <div class="carousel__item__person">
                <img src="@/assets/img/carousel/person.webp" alt="person" />
                <div class="carousel__item__person__text">
                  <h3>Johnny Andro</h3>
                  <p>Director, Company</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </VueSlickCarousel>
    </div>
  </div>
</template>

<script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
// optional style for arrows & dots
import "vue-slick-carousel/dist/vue-slick-carousel-theme.css";

export default {
  components: { VueSlickCarousel },
  data() {
    return {
      slickSettings: {
        slidesToShow: 1,
        slidesToScroll: 1,
        infinite: false,
        dots: true,
      },
    };
  },
};
</script>

<style>
</style>