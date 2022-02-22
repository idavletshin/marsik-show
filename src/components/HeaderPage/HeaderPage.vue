<template>
  <header class="header-page">
    <nav class="header-page__nav nav">
      <a href="#" class="nav__logo logo">
        <div class="logo__img">
          <img
            src="@/assets/images/confetti_2.svg"
            width="85"
            height="85"
            alt="Конфетти"
          />
        </div>
        <p class="logo__text">
          Marsik
          <br />
          Show
        </p>
      </a>
      <ul class="nav__list nav-list">
        <li class="nav-list__item nav-item">
          <a href="#" class="nav-item__link">Программы</a>
        </li>
        <li class="nav-list__item nav-item">
          <a href="#" class="nav-item__link">Цены</a>
        </li>
        <li class="nav-list__item nav-item">
          <a href="#" class="nav-item__link">Портфолио</a>
        </li>
        <li class="nav-list__item nav-item">
          <a href="#" class="nav-item__link">Отзывы</a>
        </li>
        <li class="nav-list__item nav-item">
          <a href="#" class="nav-item__link">Контакты</a>
        </li>
      </ul>
      <ul class="nav__list nav-list user-action">
        <li class="nav-list__item nav-item">
          <a
            href="tel:+79685598250"
            class="nav-item__link nav-item__link_contact"
            >+7 968 559 82 50</a
          >
        </li>
        <li class="nav-list__item nav-item">
          <a href="#" class="nav-item__link party-link-small"
            >Заказать праздник</a
          >
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "HeaderPage",
};
</script>

<style lang="scss">
.header-page,
.nav {
  display: flex;
  width: 100%;
}
.header-page__nav {
  margin: auto;
}
.nav {
  max-width: 1840px;
  padding: 40px;
}
.nav__logo {
  flex-grow: 1.5;
}
.logo {
  display: flex;
  align-items: center;
  width: 190px;
  color: $white;
  text-decoration: none;
}
.logo__img {
  width: 85px;
  height: 85px;
  margin-right: 8px;
}
.logo__text {
  font-family: $second-font;
  font-size: 30px;
  font-weight: 700;
  line-height: 30px;
  text-transform: uppercase;
}
.nav__list {
  justify-content: flex-end;
  &:not(.user-action) {
    flex-grow: 5;
  }
}
.nav-list {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}
.nav-list__item {
}
.nav-item {
}
.nav-item__link {
  display: inline-block;
  padding: 12px 20px;
  font-size: 20px;
  font-weight: 500;
  line-height: 24px;
  color: $white;
  text-decoration: none;
  text-align: center;
  transition: all 0.2s ease 0s;
  &:hover {
    color: $red;
    text-shadow: 1px 1px 10px $red;
  }
}
.nav-list.user-action {
  flex-grow: 3;
  margin-left: auto;
}
.user-action {
}
.nav-item__link_contact {
}
.party-link {
}
.nav-item__link.party-link-small {
  font-size: 14px;
  font-weight: 700;
  text-transform: uppercase;
  border: 3px solid $white;
  border-radius: 62px;

  &:hover {
    border-color: $red;
    box-shadow: 0 0 5px $red;
  }

  &:focus {
    color: $red;
  }

  &:active {
    // border-color: ;
    color: $white;
    text-shadow: unset;
    border-color: $white;
  }
}
</style>
