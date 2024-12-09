<template>
  <div class="history-item">
    <div class="content">
      <img src="../assets/images/history.png" alt="history-item" />
      <div class="text">
        <pre>
Создатель направления <b>Наталья Григорьевна Крушинская</b>  -  музыкант по образованию, приехала в Дивеево в 1991 г.

Поселившись в с. Большое Череватово неподалеку от Дивеево, Наталья Григорьевна познакомилась с  Череватовским гончарным промыслом и узнала о существовании залежей Череватовской (Дивеевской)  глины.

Тогда и начались первые опыты лепки. Наталья Григорьевна лепила сама и старалась увлечь лепкой местное население, в дальнейшем возник кружок лепки из глины.

Постепенно мастерская расширялась, учеников становилось все больше, изделия приобретали самобытный стиль
        </pre>
      </div>
    </div>
    <img src="../assets/images/toy-1.svg" alt="toy-1" class="toy-1" />
    <img src="../assets/images/toy-2.svg" alt="toy-2" class="toy-2" />
  </div>
</template>

<style lang="scss" scoped>
.history-item {
  margin-top: 176.79rem;
  position: relative;
  .content {
    display: flex;
    gap: 27rem;
    flex-direction: row;
    width: 1695.49rem;
    margin: 0 auto;

    img {
      width: 574.49rem;
      height: 100%;
      object-fit: cover;
      border-radius: 24rem;
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

      pre {
        white-space: pre-line;
        font-family: inherit;

        b {
          font-weight: 900;
        }
      }
    }
  }

  .toy-1 {
    position: absolute;
    top: -170rem;
    right: 0rem;
    width: 280.77rem;
    height: 421.15rem;
    object-fit: cover;
  }
  .toy-2 {
    position: absolute;
    bottom: -250rem;
    right: 0rem;
    width: 500.19rem;
    height: 374.66rem;
    object-fit: cover;
  }
}
</style>
