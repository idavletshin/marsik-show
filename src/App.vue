<template>
  <header-page />
  <main class="main-index">
    <div class="page-container">
      <section class="banner">
        <h1 class="banner__main-title main-title">
          Организация
          <br />
          детских
          <br />
          праздников
        </h1>
        <div class="banner__button-group">
          <a href="#" class="button party-link">Заказать праздник</a>
          <a href="#" class="button button-price">Узнать цены</a>
        </div>
      </section>
      <section class="programs">
        <h2 class="programs__title title">Программы</h2>
        <h3 class="programs__subtitle subtitle">
          Аниматоры и квесты<sup><a href="#" class="">52</a></sup>
        </h3>
        <ul class="programs__list programs-list">
          <li class="programs-list__item program-item">
            <img
              class="program-item__image"
              src="./assets/images/animators/image_1.png"
              width="330"
              height="220"
              alt=""
            />
            <h4 class="program-item__title">Загадочное происшествие</h4>
            <p class="program-item__desc">
              Вечеринка… звучит приятная музыка, собираются гости, впереди много
              поздравлений и подарков.
            </p>
          </li>
          <li class="programs-list__item program-item">
            <img
              class="program-item__image"
              src="./assets/images/animators/image_2.png"
              width="330"
              height="220"
              alt=""
            />
            <h4 class="program-item__title">Загадочное происшествие</h4>
            <p class="program-item__desc">
              Вечеринка… звучит приятная музыка, собираются гости, впереди много
              поздравлений и подарков.
            </p>
          </li>
          <li class="programs-list__item program-item">
            <img
              class="program-item__image"
              src="./assets/images/animators/image_3.png"
              width="330"
              height="220"
              alt=""
            />
            <h4 class="program-item__title">Загадочное происшествие</h4>
            <p class="program-item__desc">
              Вечеринка… звучит приятная музыка, собираются гости, впереди много
              поздравлений и подарков.
            </p>
          </li>
          <li class="programs-list__item program-item">
            <img
              class="program-item__image"
              src="./assets/images/animators/image_1.png"
              width="330"
              height="220"
              alt=""
            />
            <h4 class="program-item__title">Загадочное происшествие</h4>
            <p class="program-item__desc">
              Вечеринка… звучит приятная музыка, собираются гости, впереди много
              поздравлений и подарков.
            </p>
          </li>
          <li class="programs-list__item program-item">
            <img
              class="program-item__image"
              src="./assets/images/animators/image_2.png"
              width="330"
              height="220"
              alt=""
            />
            <h4 class="program-item__title">Загадочное происшествие</h4>
            <p class="program-item__desc">
              Вечеринка… звучит приятная музыка, собираются гости, впереди много
              поздравлений и подарков.
            </p>
          </li>
        </ul>
      </section>
      <section class="experience">
        <h2 class="experience__title title">Опыт команды</h2>
        <p class="experience__description">
          Самые яркие и необычные детские праздники у нас! Мы - команда молодых
          и очень энергичных аниматоров - предлагаем вам довериться
          профессионалам и подарить своим детям настоящую сказку!
        </p>
        <ul class="experience__list experience-list">
          <li class="experience-list__item">
            <p class="experience-item__num">60</p>
            <p class="experience-item__text">
              Автор
              <br />
              ских программ
            </p>
          </li>
          <li class="experience-list__item">
            <p class="experience-item__num">55</p>
            <p class="experience-item__text">
              Персона
              <br />
              жей на выбор
            </p>
          </li>
          <li class="experience-list__item">
            <p class="experience-item__num">5<sup>лет</sup></p>
            <p class="experience-item__text">Опыт работы</p>
          </li>
        </ul>
      </section>
      <section class="reviews"></section>
    </div>
  </main>
  <footer-page />
</template>

<script>
import HeaderPage from "@/components/HeaderPage/HeaderPage";
import FooterPage from "@/components/FooterPage/FooterPage";

export default {
  components: {
    HeaderPage,
    FooterPage,
  },
};
</script>

<style lang="scss">
#app {
  display: flex;
  flex-direction: column;
  height: 100%;
}
main {
  flex-grow: 1;
}
.main-index {
  position: relative;
  padding-top: 30px;
  &:before {
    position: absolute;
    content: "";
    top: -100px;
    left: -230px;
    width: 1080px;
    height: 500px;
    background-image: url("./assets/images/vector_4.svg");
    background-position: center;
    background-repeat: no-repeat;
    background-size: contain;
    z-index: -1;
  }

  &:after {
    position: absolute;
    content: "";
    right: -150px;
    top: 350px;
    width: 584px;
    height: 929px;
    background-image: url("./assets/images/vector_3.svg");
    background-position: center;
    background-repeat: no-repeat;
    background-size: contain;
    z-index: -1;
  }
}

.banner {
  position: relative;
  display: flex;
  flex-direction: column;
  width: 100%;
  margin-bottom: 100px;
  &::after {
    position: absolute;
    content: "";
    right: 0;
    bottom: -65px;
    width: 512px;
    height: 512px;
    background-image: url("./assets/images/confetti_1.svg");
    background-position: center;
    background-repeat: no-repeat;
    background-size: 100%;
    z-index: -1;
  }
}
.banner__main-title {
  margin-bottom: 80px;
}
.banner__button-group {
  .button {
    margin-bottom: 25px;
  }
  .button:not(:last-child) {
    margin-right: 25px;
  }
}
.button {
}
.party-link {
}
.button-price {
}

.programs {
}
.programs__subtitle {
  margin-bottom: 32px;
  sup {
    font-size: 18px;
    line-height: 27px;
    color: $yellow;
  }
}
.programs__list {
  display: flex;
  flex-wrap: wrap;
}
.programs-list {
}
.programs-list__item {
}
.program-item {
  flex-basis: 25%;
}
.program-item__image {
}
.program-item__title {
}
.program-item__desc {
}
.experience {
  margin-bottom: 100px;
}
.experience__title {
  margin-bottom: 64px;
}
.experience__description {
  margin-bottom: 96px;
  font-size: 36px;
  font-weight: 500;
  line-height: 49px;
  text-align: center;
}
.experience__list {
}
.experience-list {
  display: flex;
  justify-content: space-between;
}
.experience-list__item {
  flex-basis: 33%;
  word-break: break-word;
  margin-bottom: 25px;
}
.experience-item__num {
  font-family: $third-font;
  font-size: 200px;
  font-weight: 700;
  line-height: 200px;
  sup {
    position: relative;
    top: 24px;
    vertical-align: top;
    font-size: 24px;
    line-height: 24px;
  }
}
.experience-item__text {
  font-size: 80px;
  font-weight: 900;
  line-height: 80px;
}
.experience-list__item:nth-child(1) .experience-item__text {
  color: $green;
}
.experience-list__item:nth-child(2) .experience-item__text {
  color: $orange-200;
}
.experience-list__item:nth-child(3) .experience-item__text {
  color: $red;
}
</style>
