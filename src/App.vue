<template>
  <div id="app">
    <div class="wrapper">
      <div class="container">
        <header :class="$style.header">
          <router-link to="/" :class="$style.backLink">
            <ArrowIcon />
          </router-link>
          <div :class="$style.pageTitle">Мои списки</div>
          <div :class="$style.controlls">
            <button :class="$style.crossIcon" type="button">
              <CrossIcon />
            </button>
            <button type="button">
              <MoreIcon />
            </button>
          </div>
        </header>
        <router-view />
      </div>
      <footer :class="$style.footer">
        <div :class="[$style.footerContainer, 'container']">
          <ul :class="$style.btns">
            <li :class="$style.btnItem">
              <QuotesIcon />
              <span>Quotes</span>
            </li>
            <li :class="$style.btnItem">
              <ProtfolioIcon />
              <span>Protfolio</span>
            </li>
            <li :class="$style.btnItem">
              <LampIcon />
              <span>Ideas</span>
            </li>
            <li :class="$style.btnItem">
              <RocketIcon />
              <span>IPO</span>
            </li>
            <li :class="$style.btnItem">
              <MenuIcon />
              <span>Menu</span>
            </li>
          </ul>
        </div>
      </footer>
    </div>
  </div>
</template>

<script>
import ArrowIcon from "./components/icons/ArrowIcon.vue";
import MoreIcon from "./components/icons/MoreIcon.vue";
import CrossIcon from "./components/icons/CrossIcon.vue";
import LampIcon from "./components/icons/LampIcon.vue";
import ProtfolioIcon from "./components/icons/ProtfolioIcon.vue";
import RocketIcon from "./components/icons/RocketIcon.vue";
import QuotesIcon from "./components/icons/QuotesIcon.vue";
import MenuIcon from "./components/icons/MenuIcon.vue";
export default {
  name: "App",
  components: {
    ArrowIcon,
    MoreIcon,
    CrossIcon,
    LampIcon,
    ProtfolioIcon,
    RocketIcon,
    QuotesIcon,
    MenuIcon,
  },
};
</script>

<style lang="scss" module>
.header {
  display: flex;
  justify-content: space-between;
  padding: 9px 16px;
  background: #fff;
}

.pageTitle {
  font-size: 17px;
  line-height: 22px;
  letter-spacing: -0.408px;
  color: $gray-800;
}

.crossIcon {
  margin-right: 19px;
}

.footer {
  margin-top: auto;
}

.footerContainer {
  background-color: #fff;

  &::before {
    content: "";
    display: block;
    width: 100%;
    height: 1px;
    background-color: #9ca3af;
  }
}

.btns {
  display: flex;
  justify-content: space-between;
}

.btnItem {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  margin-top: 9px;
  padding: 0 16px 8px 16px;
  font-weight: 500;
  font-size: 10px;
  line-height: 12px;
  letter-spacing: -0.24px;
  transition: all 0.3s;
  cursor: pointer;

  &:hover {
    color: $system-blue;
  }
}

.btnItem svg {
  transition: fill 0.3s;
}
.btnItem:hover svg {
  fill: $system-blue;
}
</style>
