<script setup></script>

<template>
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
</template>

<style scoped lang="scss">
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
  --bs-accordion-btn-icon: url(../assets/images/plus.svg);
  --bs-accordion-btn-active-icon: url(../assets/images/minus.svg);
}
</style>
