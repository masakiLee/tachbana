<script setup>
import conceptProImgOne from "../assets/images/conceptProImgOne.jpg";
import conceptProImgTwo from "../assets/images/conceptProImgTwo.jpg";
import conceptProImgThree from "../assets/images/conceptProImgThree.jpg";
import conceptProImgFour from "../assets/images/conceptProImgFour.jpg";
import conceptProImgFive from "../assets/images/conceptProImgFive.jpg";
</script>

<template>
  <section class="concept">
    <div class="container">
      <div class="row">
        <div class="col-md-4 pt-6 pt-md-8 pb-0 pb-md-8">
          <div class="conceptSticky d-flex">
            <div class="conceptMain">
              <h2 class="concept-title text-vertical">橘鮨理念</h2>
            </div>
            <h3 class="concept-text mt-5 ms-3 ms-md-7">
              選用新鮮食材 最適合的調理方式 並以精美刀工 盛裝的器皿融合色彩
              平衡呈現於盤上 享用美食同時 欣賞到精緻的藝術品
            </h3>
          </div>
        </div>
        <div class="col-md-8">
          <ul class="conceptPro">
            <li class="d-none d-md-block">
              <img
                :src="conceptProImgOne"
                alt="conceptProImgOne"
                class="conceptProImg"
              />
            </li>
            <li>
              <img
                :src="conceptProImgTwo"
                alt="conceptProImgTwo"
                class="conceptProImg"
              />
            </li>
            <li>
              <img
                :src="conceptProImgThree"
                alt="conceptProImgThree"
                class="conceptProImg"
              />
            </li>
            <li class="d-none d-md-block">
              <img
                :src="conceptProImgFour"
                alt="conceptProImgFour"
                class="conceptProImg"
              />
            </li>
            <li class="d-none d-md-block">
              <img
                :src="conceptProImgFive"
                alt="conceptProImgFive"
                class="conceptProImg"
              />
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
.concept {
  &Sticky {
    position: sticky;
    top: 120px;
  }
  &-title {
    border: 3px solid #f25c05;
  }
  &-text {
    word-break: keep-all;
    line-height: 64px;
    letter-spacing: 6px;
    @media (max-width: 768px) {
      line-height: 48px;
    }
  }
  li {
    width: 50%;
    padding: 240px 0;
    &:nth-child(odd) {
      margin-left: auto;
      @media (max-width: 576px) {
        padding: 0 0 24px 0;
      }
    }
    @media (max-width: 768px) {
      width: 100%;
      padding: 24px 0;
    }
  }
  &Pro {
    position: relative;
    border-left: 1px solid #262626;
    border-right: 1px solid #262626;
    @media (max-width: 768px) {
      border-left: none;
      border-right: none;
    }

    &::after {
      content: "";
      display: block;
      width: 1px;
      height: 100%;
      background-color: #262626;
      position: absolute;
      top: 0;
      left: 50%;

      @media (max-width: 768px) {
        display: none;
      }
    }
    &Img {
      aspect-ratio: 367/231;
      object-fit: cover;
    }
  }
}
</style>
