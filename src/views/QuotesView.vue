<template>
  <div :class="$style.quotes">
    <div :class="$style.heading">Избранное</div>
    <ul :class="$style.quotesList">
      <QuotesItem v-for="n in 5" :key="n" />
    </ul>
  </div>
</template>

<script>
import QuotesItem from "../components/QuotesItem.vue";
export default {
  name: "QuotesView",

  components: {
    QuotesItem,
  },
};
</script>

<style lang="scss" module>
.quotes {
  flex: 1;
  max-height: calc(100vh - 96px);
  overflow-y: auto;
  background-color: #fff;
}

.heading {
  padding: 9px 16px;
  font-weight: 600;
  font-size: 22px;
  line-height: 28px;
}

.quotesList {
  padding: 9px 16px 0 16px;
}
</style>
