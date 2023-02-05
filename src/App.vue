<script setup></script>

<template>
  <header class="header d-flex justify-content-between align-items-center">
    <a href="#" class="hamburgerBtn">
      <span class="hamburgerLine"></span>
      <span class="hamburgerLine"></span>
      <span class="hamburgerLine"></span>
    </a>
    <h1>
      <a href="#">
        <img src="./assets/images/logo.svg" alt="橘鮨" class="logo" />
      </a>
    </h1>
    <a href="#" class="shoppingBtn">
      <img
        src="./assets/images/shopping.svg"
        alt="購物車"
        class="shoppingCar"
      />
    </a>
  </header>
  <div class="container">
    <div class="row justify-content-center">
      <div class="col-md-10 banner">
        <img
          src="./assets/images/bannerOne.jpg"
          alt=""
          class="rounded-3 bannerImg mx-auto"
        />
        <div class="subtitle subtitleOne text-white bg-dark">その瞬間だけ</div>
        <div class="subtitle subtitleTwo text-white bg-dark">味わえる</div>
        <div class="subtitle subtitleThree text-white bg-dark">
          一期一会の逸品
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.logo {
  padding: 8px 0;
}

.hamburgerLine {
  width: 32px;
  height: 4px;
  background-color: #fff;
  border-radius: 4px;
  display: block;
}

.hamburgerLine:nth-child(2) {
  margin: 10px 0;
}
.hamburgerBtn,
.shoppingBtn {
  width: 96px;
  display: block;
  padding: 32px;
}

.banner {
  margin-top: 40px;
  position: relative;
}

.subtitle {
  writing-mode: vertical-lr;
  padding: 16px;
  letter-spacing: 12px;
}

.subtitleOne {
  box-shadow: 3px 3px 1px #f25c05;
  position: absolute;
  top: -24px;
  right: -20px;
}
.subtitleTwo {
  box-shadow: -3px 3px 1px #f25c05;
  position: absolute;
  top: 96px;
  right: 48px;
}
.subtitleThree {
  box-shadow: -3px 3px 1px #f25c05;
  position: absolute;
  bottom: -24px;
  left: -24px;
}
</style>
