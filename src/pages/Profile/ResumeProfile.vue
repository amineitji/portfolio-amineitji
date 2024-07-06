<!-- eslint-disable vue/no-mutating-props -->
<template>
  <card>
  <img src="/img/cv_portfolio_fr.png" alt="CV" class="cv-image" @load="adjustCardWidth" ref="cvImage" />
    <h5 slot="header" class="title">Mon CV</h5>
    <div class="row">
      <div class="col-md-5 pr-md-1">
      </div>
      <div class="col-md-3 px-md-1">
      </div>
      <div class="col-md-4 pl-md-1">
      </div>
    </div>
    <div class="row">
      <div class="col-md-6 pr-md-1">
      </div>
      <div class="col-md-6 pl-md-1">
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
      </div>
    </div>
    <div class="row">
      <div class="col-md-4 pr-md-1">
      </div>
      <div class="col-md-4 px-md-1">
      </div>
      <div class="col-md-4 pl-md-1">
      </div>
    </div>
    <div class="row">
      <div class="col-md-8">
      </div>
    </div>
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