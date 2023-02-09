<script setup></script>

<template>
  <section class="newsSection d-flex align-items-center">
    <div class="container">
      <div class="row">
        <div class="col-md-4">
          <h2 class="text-vertical newsSection-title mx-auto">最新消息</h2>
        </div>
        <div class="col-md-8 d-flex flex-column justify-content-between px-5">
          <a
            href="#"
            class="d-flex flex-column justify-content-around flex-grow-1 my-4"
          >
            <h3 class="mb-3 mb-md-0">2023.01.25</h3>
            <h3>慶開幕輸入折扣碼享優惠</h3>
          </a>
          <a href="#" class="text-end">看更多...</a>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
.newsSection {
  height: 254px;
  background-color: rgba(0, 0, 0, 0.6);
  // 設置背景混和模式為相乘模式
  background-blend-mode: multiply;
  background-image: url(./assets/images/newsBackground.jpg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  @media (max-width: 768px) {
    height: 420px;
  }
  &-title {
    border: 3px solid #f25c05;
  }
}
</style>
