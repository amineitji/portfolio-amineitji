<template>
  <div class="card" ref="card">
    <div class="card-header">
      <h5 class="title">CV</h5>
      <p>
        Vous pouvez me contacter directement sur mon
        <a href="https://www.linkedin.com/in/amine-itji-5a8696268/">LinkedIn - Amine ITJI</a>
      </p>
    </div>
    <div class="card-body">
      <img src="/img/cv_portfolio_fr.png" alt="CV" class="cv-image" @load="adjustCardWidth" ref="cvImage" />
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    adjustCardWidth() {
      const image = this.$refs.cvImage;
      const card = this.$refs.card;
      if (image && card) {
        const aspectRatio = image.naturalWidth / image.naturalHeight;
        const newWidth = window.innerHeight * aspectRatio;
        card.style.width = `${newWidth}px`;
      }
    }
  },
  mounted() {
    window.addEventListener('resize', this.adjustCardWidth);
  },
  beforeDestroy() {
    window.removeEventListener('resize', this.adjustCardWidth);
  }
};
</script>

<style>
.card {
  margin: 0 auto;
}

.card-body {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 0;
  margin: 0;
}

.cv-image {
  height: 100vh; /* Full viewport height */
  width: auto; /* Maintain aspect ratio */
  display: block;
}
</style>
