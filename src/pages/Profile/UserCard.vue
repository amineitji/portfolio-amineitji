<template>
  <card type="user">
    <p class="card-text"></p>
    <div class="author">
      <div class="block block-one"></div>
      <div class="block block-two"></div>
      <div class="block block-three"></div>
      <div class="block block-four"></div>
      <a class="user-link" href="#">
        <img class="avatar" src="img/anime3.png" alt="..." />
        <h5 class="title">{{ user.fullName }}</h5>
      </a>
      <p class="description">
        {{ user.title }}
      </p>
    </div>
    <p></p>
    <p class="card-description">
      {{ user.description }}
    </p>
    <div slot="footer" class="button-container">
      <base-button tag="a" href="https://www.linkedin.com/in/amine-itji-5a8696268/" target="_blank"><i class="fab fa-linkedin"></i></base-button>
      <base-button tag="a" href="https://github.com/amineitji" target="_blank"><i class="fab fa-github"></i></base-button>
      <base-button tag="a" href="https://mail.google.com/mail/u/amineitji@gmail.com/?view=cm&to=amineitji@gmail.com" target="_blank"><i class="fab fa-google-plus"></i></base-button>
    </div>
  </card>
</template>

<script>
export default {
  props: {
    user: {
      type: Object,
      default: () => {
        return {};
      },
    },
  },
};
</script>

<style>
.user-link {
  display: block;
  width: 100%;
}
</style>
