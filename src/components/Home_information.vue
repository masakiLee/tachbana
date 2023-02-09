<script setup>
import logo from "../assets/images/logo.svg";
import logoSm from "../assets/images/logo-sm.svg";
</script>

<template>
  <section class="information py-5">
    <div class="container">
      <div class="d-flex flex-column flex-md-row align-items-center">
        <div class="col-md-4 mb-4 mb-md-0">
          <img
            :src="logo"
            alt="橘 Tachibana"
            class="logoImg d-none d-md-block"
          />
          <img
            :src="logoSm"
            alt="橘 Tachibana"
            class="logoImg d-block d-md-none"
          />
        </div>
        <div class="col-md-8">
          <ul class="informationList px-4">
            <li class="mb-2">
              <p class="informationListName">地址</p>
              <p>新北市板橋區縣民大道一段22號</p>
            </li>
            <li class="mb-2">
              <p class="informationListName">電話</p>
              <p>02-2999-9999</p>
            </li>
            <li class="mb-2">
              <p class="informationListName">營業時間</p>
              <p>11:30~14:00 17:00~21:00</p>
            </li>
            <li>
              <p class="informationListName">公休日</p>
              <p>週三</p>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
.information {
  height: 344px;
  background-color: rgba(0, 0, 0, 0.6);
  // 設置背景混和模式為相乘模式
  background-blend-mode: multiply;
  background-image: url(../assets/images/informationImg.jpg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  font-size: 20px;
  @media (max-width: 992px) {
    height: 404px;
  }
  @media (max-width: 768px) {
    height: 524px;
  }
}
</style>
