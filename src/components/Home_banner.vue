<script>
import { Swiper, SwiperSlide } from "swiper/vue";
import { Autoplay, Pagination } from "swiper";

// Import Swiper styles
import "swiper/css";
import "swiper/css/navigation";
import "swiper/css/pagination";

export default {
  data() {
    return {
      modules: [Autoplay, Pagination],
    };
  },
  components: {
    Swiper,
    SwiperSlide,
  },
};
</script>
<template>
  <div class="mt-4 mb-7 mb-md-9 pt-6">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-md-10 banner">
          <swiper
            id="swiper"
            :slides-per-view="1"
            :space-between="50"
            :modules="modules"
            :autoplay="{
              delay: 8000,
              disableOnInteraction: false,
            }"
            :pagination="{ clickable: true }"
          >
            <swiper-slide>
              <img
                class="bannerImg mx-auto"
                src="../assets/images/bannerOne.jpg"
                alt=""
              />
            </swiper-slide>
            <swiper-slide>
              <img
                class="bannerImg mx-auto"
                src="../assets/images/bannerTwo.jpg"
                alt=""
              />
            </swiper-slide>
            <swiper-slide>
              <img
                class="bannerImg mx-auto"
                src="../assets/images/bannerThree.jpg"
                alt=""
              />
            </swiper-slide>
          </swiper>
          <h2 class="subtitle subtitleOne text-vertical bg-dark">
            その瞬間だけ
          </h2>
          <h2 class="subtitle subtitleTwo text-vertical bg-dark text-nowrap">
            味わえる
          </h2>
          <h2 class="subtitle subtitleThree text-vertical bg-dark">
            一期一会の逸品
          </h2>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped lang="scss">
.banner {
  margin-top: 40px;
  position: relative;
}

.subtitle {
  z-index: 5;
  &One {
    box-shadow: 3px 3px 1px #f25c05;
    position: absolute;
    top: -24px;
    right: -20px;
    @media (max-width: 768px) {
      top: -48px;
      right: 16px;
    }
  }
  &Two {
    box-shadow: -3px 3px 1px #f25c05;
    position: absolute;
    top: 96px;
    right: 36px;
    @media (max-width: 768px) {
      top: 48px;
      right: 66px;
    }
  }
  &Three {
    box-shadow: -3px 3px 1px #f25c05;
    position: absolute;
    bottom: -24px;
    left: -24px;
    @media (max-width: 768px) {
      bottom: -48px;
      left: 16px;
    }
  }
}
.swiper {
  width: 100%;
  height: 567px;
}
.swiper-slide img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
  padding-bottom: 24px;
}
:deep(.swiper-pagination) {
  text-align: end;
  bottom: -4px;
}

:deep(.swiper-pagination)
  .swiper-pagination-bullet.swiper-pagination-bullet-active {
  background-color: #f25c05;
}
:deep(.swiper-pagination-bullet) {
  background-color: #262626;
}
.swiper-horizontal > .swiper-pagination-bullets .swiper-pagination-bullet,
:deep(.swiper-pagination-horizontal.swiper-pagination-bullets)
  .swiper-pagination-bullet {
  width: 48px;
  height: 8px;
  border-radius: 0;
  margin: 0 0 0 8px;
}
</style>
