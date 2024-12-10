<template>
  <div class="features-item">
    <div class="text">
      <h2>ОСОБЕННОСТИ ИЗГОТОВЛЕНИЯ</h2>
      <pre>
        Одной из особенностей дивеевской игрушки – это цветовая гамма изделия. Та местность, где зародилась игрушка, уникальна. Там встречаются глины от белой и лиловой до оранжевой и даже тёмно-бордовой. Многообразие цвета натуральной глины добавили колорит, яркость, праздничное настроение работам. Именно они позволили создавать удивительные произведения без каких-либо красителей или глазурей, декорируя игрушки при помощи красной, розовой и белой глин.

Но красота и уникальность дивеевской игрушки не только в цвете, но и в необычном рельефном оформлении. Это достигается всевозможными вдавлениями, элементами лепнины, процарапыванием узоров, начертаниями, графическим рисунком, часто с помощью обычных подручных средств. В ход идут и колпачки от фломастеров, и стержни, и т.п.
      </pre>
    </div>
    <div class="images">
      <img src="@/assets/images/feature-1.webp" alt="features-img-1" class="img-1" />
      <img src="@/assets/images/feature-2.webp" alt="features-img-2" class="img-2" />
      <img src="@/assets/images/feature-3.webp" alt="features-img-3" class="img-3" />
      <img src="@/assets/images/feature-4.webp" alt="features-img-4" class="img-4" />
    </div>
  </div>
</template>

<style lang="scss" scoped>
.features-item {
  margin-top: 160.5rem;

  .text {
    width: 1303rem;
    margin: 0 auto;
    background-color: $secondary-color;
    padding: 80rem;
    border-radius: 24rem;

    h2 {
      font-size: 80rem;
      line-height: 96rem;
      font-family: 'Condensed';
      color: $primary-color;
      text-align: center;
    }

    pre {
      margin-top: 31rem;
      font-size: 20rem;
      line-height: 24.2rem;
      font-family: 'Inter';
      white-space: pre-line;
      font-family: inherit;
      text-align: center;
      color: $text-color;
    }
  }

  .images {
    position: relative;
    width: 100%;
    height: 618.51rem;

    img {
      border-radius: 24rem;
      position: absolute;
    }

    .img-1 {
      width: 498.7rem;
      height: 618.51rem;
      top: 70rem;
      left: -250rem;
      transform: rotate(-15deg);
    }
    .img-2 {
      width: 509.71rem;
      height: 338.44rem;
      top: 150rem;
      left: 358rem;
      transform: rotate(3.96deg);
    }
    .img-3 {
      width: 440.2rem;
      height: 399.73rem;
      top: 170rem;
      left: 936.9rem;
      transform: rotate(-4.94deg);
    }
    .img-4 {
      width: 498.7rem;
      height: 618.51rem;
      top: -15rem;
      left: 1500rem;
      transform: rotate(9.32deg);
    }
  }
}
</style>
