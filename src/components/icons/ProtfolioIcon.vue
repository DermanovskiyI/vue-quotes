<template>
  <div>
    <svg
      :class="$style.icon"
      width="20"
      height="20"
      viewBox="0 0 20 20"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <path
        d="M9.33867 0.507751C4.67627 0.893352 0.9649 4.60473 0.5793 9.26713H9.33867V0.507751ZM10.9387 0.507751V9.73588L17.4652 16.2624C18.8804 14.5896 19.7387 12.4303 19.7387 10.0671C19.7387 5.03513 15.8651 0.915753 10.9387 0.507753V0.507751ZM0.5793 10.8671C0.9873 15.7935 5.10668 19.6671 10.1387 19.6671C12.5019 19.6671 14.6612 18.8089 16.334 17.3937L9.80742 10.8671H0.5793Z"
      />
    </svg>
  </div>
</template>

<script>
export default {
  name: "PortfolioIcon",
};
</script>

<style lang="scss" module>
.icon {
  fill: #9ca3af;
}
</style>
