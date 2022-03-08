<template>
  <li :class="$style.quotesItem">
    <div :class="$style.top">
      <div :class="$style.left">
        <div :class="$style.logo">
          <img src="../static/stub/teslaIcon.png" alt="logo" />
        </div>
        <div :class="$style.name">FRHC.US</div>
        <div :class="$style.position"><span>long</span></div>
        <div :class="$style.priceChange"><span>TP</span></div>
      </div>
      <div :class="$style.right">
        <div :class="$style.price"><span>51.80</span></div>
      </div>
    </div>
    <div :class="$style.bottom">
      <div :class="$style.info">
        <div :class="$style.market">NASDAQ</div>
        <div>FREEDOM HOLDING CORP-NV</div>
      </div>
      <div :class="$style.percents">
        <div :class="$style.percent">0.00%</div>
        <div :class="$style.percent">0.00%</div>
      </div>
    </div>
  </li>
</template>

<script>
export default {
  name: "QuotesItem",
};
</script>

<style lang="scss" module>
.quotesItem {
  display: flex;
  flex-direction: column;
  padding-bottom: 8px;
  text-transform: uppercase;
  font-size: 17px;
  line-height: 22px;
  letter-spacing: -0.408px;
  color: $gray-800;

  &::before {
    content: "";
    display: block;
    width: 100%;
    height: 1px;
    margin-bottom: 10px;
    background: #e5e7eb;
  }
}

.top {
  display: flex;
  align-items: center;
  margin-bottom: 8px;
}

.left {
  display: flex;
  align-items: center;
  column-gap: 10px;
}

.logo {
  display: flex;
  flex-shrink: 0;
}

.position {
  display: flex;
  align-items: center;
  padding: 2px 4px;
  border-radius: 8px;
  background: $system-blue;
  color: #fff;
  font-size: 10px;
  font-weight: 600;
  line-height: 13px;
}

.priceChange {
  display: flex;
  align-items: center;
  padding: 2px 4px;
  border: 1px solid $system-green;
  border-radius: 8px;
  color: $system-green;
  font-size: 10px;
  font-weight: 600;
  line-height: 13px;
}

.right {
  margin-left: auto;
}

.price {
  display: flex;
  align-items: center;
  padding: 2px 4px;
  border-radius: 8px;
  background: $system-green;
  color: #fff;
  font-size: 17px;
  line-height: 22px;
}

.bottom {
  display: flex;
  align-items: center;
}

.info {
  display: flex;
  color: $gray-500;
  font-size: 13px;
  line-height: 18px;
  letter-spacing: -0.078px;
}

.market {
  display: flex;
  align-items: center;

  &::after {
    content: "";
    display: block;
    width: 1px;
    height: 100%;
    margin: 0 10px;
    background: #e5e7eb;
  }
}

.percents {
  display: flex;
  column-gap: 8px;
  margin-left: auto;
  font-size: 13px;
  line-height: 18px;
  letter-spacing: -0.078px;
}
</style>
