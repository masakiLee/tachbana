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
        <img
          src="./assets/images/logo.svg"
          alt="橘 Tachibana"
          class="logoImg"
        />
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
  <div class="mt-4 mb-7 mb-md-9">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-md-10 banner">
          <img
            src="./assets/images/bannerOne.jpg"
            alt=""
            class="rounded-3 bannerImg mx-auto"
          />
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
  <main>
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
    <section class="concept">
      <div class="container">
        <div class="row">
          <div class="col-md-4 pt-6 pt-md-8 pb-0 pb-md-8">
            <div class="conceptSticky d-flex">
              <div class="conceptMain">
                <h2 class="concept-title text-vertical">橘鮨理念</h2>
              </div>
              <h3 class="concept-text mt-5 ms-4 ms-md-7">
                選用新鮮食材 最適合的調理方式 並以精美刀工 盛裝的器皿融合色彩
                平衡呈現於盤上 享用美食同時 欣賞到精緻的藝術品
              </h3>
            </div>
          </div>
          <div class="col-md-8">
            <ul class="conceptPro">
              <li class="d-none d-md-block">
                <img
                  src="./assets/images/conceptProImgOne.jpg"
                  alt="conceptProImgOne"
                  class="conceptProImg"
                />
              </li>
              <li>
                <img
                  src="./assets/images/conceptProImgTwo.jpg"
                  alt="conceptProImgTwo"
                  class="conceptProImg"
                />
              </li>
              <li>
                <img
                  src="./assets/images/conceptProImgThree.jpg"
                  alt="conceptProImgThree"
                  class="conceptProImg"
                />
              </li>
              <li class="d-none d-md-block">
                <img
                  src="./assets/images/conceptProImgFour.jpg"
                  alt="conceptProImgFour"
                  class="conceptProImg"
                />
              </li>
              <li class="d-none d-md-block">
                <img
                  src="./assets/images/conceptProImgFive.jpg"
                  alt="conceptProImgFive"
                  class="conceptProImg"
                />
              </li>
            </ul>
          </div>
        </div>
      </div>
    </section>
    <section class="menu">
      <div class="container-fluid">
        <div class="row">
          <div class="col-xl-6 g-0 order-2 order-xl-1 d-none d-md-block">
            <ul class="menuImgBox d-flex flex-wrap">
              <li class="menuImgList">
                <div class="menuHover d-flex align-items-center pt-3 pt-lg-5">
                  <p>單品</p>
                </div>
                <img src="./assets/images/menuOne.jpg" alt="" class="menuImg" />
              </li>
              <li class="menuImgList">
                <div class="menuHover d-flex align-items-center pt-3 pt-lg-5">
                  <p>軍艦</p>
                </div>
                <img src="./assets/images/menuTwo.jpg" alt="" class="menuImg" />
              </li>
              <li class="menuImgList">
                <div class="menuHover d-flex align-items-center pt-3 pt-lg-5">
                  <p>套餐</p>
                </div>
                <img
                  src="./assets/images/menuThree.jpg"
                  alt=""
                  class="menuImg"
                />
              </li>
              <li class="menuImgList">
                <div class="menuHover d-flex align-items-center pt-3 pt-lg-5">
                  <p>捲物</p>
                </div>
                <img
                  src="./assets/images/menuFour.jpg"
                  alt=""
                  class="menuImg"
                />
              </li>
            </ul>
          </div>
          <div
            class="col-xl-6 border border-white border-2 bg-darkTwo d-flex flex-column justify-content-center order-1 order-xl-2"
          >
            <div class="menuMain py-6">
              <h2 class="menuTitle text-vertical mx-auto">美味菜單</h2>
              <h3 class="menuText text-center my-5">
                橘鮨不僅提供美味的季節性魚類 融入創意理念 透過巧手變成創意壽司
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
    <section class="fqa py-6 py-md-8">
      <div class="container">
        <h2 class="fqa-title mx-auto text-vertical">常見問題</h2>
        <div class="row justify-content-center mt-5">
          <div class="col-10 col-lg-6">
            <div class="accordion mb-4" id="accordionExampleOne">
              <div class="accordion-item border border-3 border-white">
                <h3 class="accordion-header" id="headingOne">
                  <button
                    class="accordion-button collapsed text-white text-nowrap"
                    type="button"
                    data-bs-toggle="collapse"
                    data-bs-target="#collapseOne"
                    aria-expanded="false"
                    aria-controls="collapseOne"
                  >
                    <span class="fqa-list me-4">01</span> 有推薦的壽司？
                  </button>
                </h3>
                <div
                  id="collapseOne"
                  class="accordion-collapse collapse"
                  aria-labelledby="headingOne"
                  data-bs-parent="#accordionExampleOne"
                >
                  <div class="accordion-body text-white bg-darkTwo">
                    壽司師傅精心挑選新鮮食材，可以嘗試不同的組合，品嘗我們的美味饗宴。
                  </div>
                </div>
              </div>
            </div>
            <div class="accordion mb-4" id="accordionExampleTwo">
              <div class="accordion-item border border-3 border-white">
                <h3 class="accordion-header" id="headingTwo">
                  <button
                    class="accordion-button collapsed text-white text-nowrap"
                    type="button"
                    data-bs-toggle="collapse"
                    data-bs-target="#collapseTwo"
                    aria-expanded="false"
                    aria-controls="collapseTwo"
                  >
                    <span class="fqa-list me-4">02</span> 有什麼素食選擇？
                  </button>
                </h3>
                <div
                  id="collapseTwo"
                  class="accordion-collapse collapse"
                  aria-labelledby="headingTwo"
                  data-bs-parent="#accordionExampleTwo"
                >
                  <div class="accordion-body text-white bg-darkTwo">
                    可選擇稻荷壽司，酪梨壽司...
                  </div>
                </div>
              </div>
            </div>
            <div class="accordion" id="accordionExampleThree">
              <div class="accordion-item border border-3 border-white">
                <h3 class="accordion-header" id="headingThree">
                  <button
                    class="accordion-button collapsed text-white text-nowrap"
                    type="button"
                    data-bs-toggle="collapse"
                    data-bs-target="#collapseThree"
                    aria-expanded="false"
                    aria-controls="collapseThree"
                  >
                    <span class="fqa-list me-4">03</span> 有無小孩的餐點？
                  </button>
                </h3>
                <div
                  id="collapseThree"
                  class="accordion-collapse collapse"
                  aria-labelledby="headingThree"
                  data-bs-parent="#accordionExampleThree"
                >
                  <div class="accordion-body text-white bg-darkTwo">
                    多種適合小孩口味的壽司，例如：甜蝦壽司、蛋壽司、茶碗蒸等...
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="information py-5">
      <div class="container">
        <div class="d-flex flex-column flex-md-row align-items-center">
          <div class="col-md-4 mb-4 mb-md-0">
            <h2>
              <img
                src="./assets/images/logo.svg"
                alt="橘鮨"
                class="logoImg mx-auto"
              />
            </h2>
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
  </main>
  <footer class="footer text-white text-center py-2">
    <p class="footer-text">Copyright © 橘鮨 2023 All Rights Reserved.</p>
  </footer>
</template>

<style scoped lang="scss">
.logoImg {
  padding: 8px 0;
}

.hamburgerLine {
  width: 32px;
  height: 4px;
  background-color: #fff;
  border-radius: 4px;
  display: block;
  &:nth-child(2) {
    margin: 10px 0;
  }
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

.concept {
  &Sticky {
    position: sticky;
    top: 40px;
  }
  &-title {
    border: 3px solid #f25c05;
  }
  &-text {
    word-break: keep-all;
    line-height: 64px;
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
    background: url(./assets/images/menuHoverOne.png) no-repeat;
    background-position: center 185%;
    background-size: contain;
  }
  &ImgList:nth-child(2) .menuHover {
    background: url(./assets/images/menuHoverTwo.png) no-repeat;
    background-position: center 230%;
    background-size: 80%;
  }
  &ImgList:nth-child(3) .menuHover {
    background: url(./assets/images/menuHoverThree.png) no-repeat;
    background-position: center 155%;
    background-size: contain;
  }
  &ImgList:nth-child(4) .menuHover {
    background: url(./assets/images/menuHoverFour.png) no-repeat;
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

.fqa {
  &-title {
    border: 3px solid #f25c05;
  }
  .accordion-body {
    font-size: 20px;
    letter-spacing: 8px;
    @media (max-width: 768px) {
      font-size: 16px;
    }
  }
  .accordion-button {
    letter-spacing: 4px;
    font-size: 20px;
    background-color: #1b1b1b;
    @media (max-width: 768px) {
      font-size: 16px;
    }
  }
  &-list {
    color: #f25c05;
    font-weight: 700;
  }
}

.accordion {
  --bs-accordion-btn-focus-box-shadow: none;
  --bs-accordion-btn-icon: url(./assets/images/plus.svg);
  --bs-accordion-btn-active-icon: url(./assets/images/minus.svg);
}

.information {
  height: 344px;
  background-color: rgba(0, 0, 0, 0.6);
  // 設置背景混和模式為相乘模式
  background-blend-mode: multiply;
  background-image: url(./assets/images/informationImg.jpg);
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

.footer-text {
  font-size: 12px;
  letter-spacing: 4px;
}
</style>
