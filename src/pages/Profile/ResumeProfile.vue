<!-- eslint-disable vue/no-mutating-props -->
<template>
  <card>
  <img src="/img/cv_portfolio_fr.png" alt="CV" class="cv-image" @load="adjustCardWidth" ref="cvImage" />
    <h5 slot="header" class="title">Mon CV</h5>
  </card>
</template>
<script>
export default {
  props: {
    model: {
      type: Object,
      default: () => {
        return {};
      },
    },
  },
};
</script>
<style></style>