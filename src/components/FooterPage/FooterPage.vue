<template>
  <footer class="footer-page">
    <div class="footer-page__container">
      <p class="footer-page__copyright">
        © 2016 - 2022 «Марсик Шоу» — все права защищены.
      </p>
      <ul class="footer-page__social-list">
        <li class="social-list__item">
          <a href="#" class="social-item__link social-item__link_vk">
            <span class="visually-hidden">ВКонтакте</span>
          </a>
        </li>
        <li class="social-list__item">
          <a href="#" class="social-item__link social-item__link_fb">
            <span class="visually-hidden">Facebook</span>
          </a>
        </li>
        <li class="social-list__item">
          <a href="#" class="social-item__link social-item__link_inst">
            <span class="visually-hidden">Instagram</span>
          </a>
        </li>
      </ul>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterPage",
};
</script>

<style lang="scss">
.footer-page {
  display: flex;
  width: 100%;
}
.footer-page__container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
  margin: auto;
  max-width: 1840px;
  padding: 40px;
}
.footer-page__copyright {
}
.footer-page__social-list {
  display: flex;
}
.social-list__item {
  &:not(:last-child) {
    margin-right: 40px;
  }
}
.social-item__link {
  display: block;
  width: 40px;
  height: 40px;
  background-position: center;
  background-repeat: no-repeat;
  transition: all 0.1s ease 0s;
  &_vk {
    background-image: url("../../assets/images/vk.svg");
  }
  &_fb {
    background-image: url("../../assets/images/facebook.svg");
  }
  &_inst {
    background-image: url("../../assets/images/instagram.svg");
  }
  &:hover {
    transform: scale(1.2);
  }
}
.visually-hidden {
}
</style>
