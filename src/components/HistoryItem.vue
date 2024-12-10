<template>
  <div class="history-item">
    <div class="img-wrapper">
      <img src="@/assets/images/history.png" alt="history-item" />
    </div>
    <div class="text">
      <pre>
Создатель направления <b>Наталья Григорьевна Крушинская</b>  -  музыкант по образованию, приехала в Дивеево в 1991 г.

Поселившись в с. Большое Череватово неподалеку от Дивеево, Наталья Григорьевна познакомилась с  Череватовским гончарным промыслом и узнала о существовании залежей Череватовской (Дивеевской)  глины.

Тогда и начались первые опыты лепки. Наталья Григорьевна лепила сама и старалась увлечь лепкой местное население, в дальнейшем возник кружок лепки из глины.

Постепенно мастерская расширялась, учеников становилось все больше, изделия приобретали самобытный стиль
      </pre>
    </div>
    <img src="@/assets/images/toy-1.svg" alt="toy-1" class="toy-1" />
    <img src="@/assets/images/toy-2.svg" alt="toy-2" class="toy-2" />
  </div>
</template>

<style lang="scss" scoped>
.history-item {
  display: flex;
  gap: 27rem;
  flex-direction: row;
  align-items: stretch;
  width: 1695.49rem;
  margin: 176.79rem auto 0;
  position: relative;

  .img-wrapper {
    flex: 0 0 574.49rem;
    display: flex;
    align-items: center;
    justify-content: center;

    img {
      width: 100%;
      border-radius: 24rem;
      object-fit: cover;
    }
  }

  .text {
    font-family: 'Inter';
    font-size: 28rem;
    line-height: 33.89rem;
    width: 1095rem;
    color: $primary-color;
    background-color: $secondary-color;
    padding: 80rem;
    border-radius: 24rem;
    flex: 1;

    pre {
      white-space: pre-line;
      font-family: inherit;

      b {
        font-weight: 900;
      }
    }
  }

  .toy-1 {
    position: absolute;
    top: -170rem;
    right: -80rem;
    width: 280.77rem;
    height: 421.15rem;
  }
  .toy-2 {
    position: absolute;
    bottom: -250rem;
    right: -110rem;
    width: 500.19rem;
    height: 374.66rem;
  }
}
</style>
