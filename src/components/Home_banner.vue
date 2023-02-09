<script setup>
import bannerOne from "@/assets/images/bannerOne.jpg";
</script>
<template>
  <div class="mt-4 mb-7 mb-md-9 pt-6">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-md-10 banner">
          <img :src="bannerOne" alt="" class="rounded-3 bannerImg mx-auto" />
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
</style>
