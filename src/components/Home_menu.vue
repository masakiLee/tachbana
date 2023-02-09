<script setup>
import menuOne from "../assets/images/menuOne.jpg";
import menuTwo from "../assets/images/menuTwo.jpg";
import menuThree from "../assets/images/menuThree.jpg";
import menuFour from "../assets/images/menuFour.jpg";
</script>

<template>
  <section class="menu">
    <div class="container-fluid">
      <div class="row">
        <div class="col-xl-6 g-0 order-2 order-xl-1 d-none d-md-block">
          <ul class="menuImgBox d-flex flex-wrap">
            <li class="menuImgList">
              <div class="menuHover d-flex align-items-center pt-3 pt-lg-5">
                <p>單品</p>
              </div>
              <img :src="menuOne" alt="" class="menuImg" />
            </li>
            <li class="menuImgList">
              <div class="menuHover d-flex align-items-center pt-3 pt-lg-5">
                <p>軍艦</p>
              </div>
              <img :src="menuTwo" alt="" class="menuImg" />
            </li>
            <li class="menuImgList">
              <div class="menuHover d-flex align-items-center pt-3 pt-lg-5">
                <p>套餐</p>
              </div>
              <img :src="menuThree" alt="" class="menuImg" />
            </li>
            <li class="menuImgList">
              <div class="menuHover d-flex align-items-center pt-3 pt-lg-5">
                <p>捲物</p>
              </div>
              <img :src="menuFour" alt="" class="menuImg" />
            </li>
          </ul>
        </div>
        <div
          class="col-xl-6 border border-white border-3 bg-darkTwo d-flex flex-column justify-content-center order-1 order-xl-2"
        >
          <div class="menuMain py-6">
            <h2 class="menuTitle text-vertical mx-auto">美味菜單</h2>
            <h3 class="menuText text-center my-5">
              橘鮨提供最時令的美味 融入創意理念 透過巧手變成創意壽司
              在享受美食的同時體驗 別樹一格的餐饗
            </h3>
            <button
              class="btn btn-outline-primary btn-lg d-block mx-auto menuBtn"
            >
              即刻品嘗
            </button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
.menu {
  &ImgList {
    width: 50%;
    position: relative;
    writing-mode: vertical-lr;
    .menuHover {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      height: 80%;
      width: 80%;
      border: 3px solid white;
      z-index: 2;
    }
    @media (max-width: 1200px) {
      width: 25%;
    }
  }
  &ImgList:nth-child(1) .menuHover {
    background: url(../assets/images/menuHoverOne.png) no-repeat;
    background-position: center 185%;
    background-size: contain;
  }
  &ImgList:nth-child(2) .menuHover {
    background: url(../assets/images/menuHoverTwo.png) no-repeat;
    background-position: center 230%;
    background-size: 80%;
  }
  &ImgList:nth-child(3) .menuHover {
    background: url(../assets/images/menuHoverThree.png) no-repeat;
    background-position: center 155%;
    background-size: contain;
  }
  &ImgList:nth-child(4) .menuHover {
    background: url(../assets/images/menuHoverFour.png) no-repeat;
    background-position: center 180%;
    background-size: contain;
  }

  &Img {
    aspect-ratio: 1/1;
    object-fit: cover;
    opacity: 0.3;
  }
  &Title {
    border: 3px solid #f25c05;
  }
  &Text {
    word-break: keep-all;
    line-height: 36px;
  }
  &Btn {
    letter-spacing: 12px;
    padding-left: 24px;
  }
}
</style>
