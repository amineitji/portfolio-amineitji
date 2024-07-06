<template>
  <div class="row">
    <div class="col-md-8">
      <edit-profile-form :model="model"> </edit-profile-form>
    </div>
    <div class="col-md-4">
      <user-card :user="user"></user-card>
    </div>
  </div>
</template>

<script>
import EditProfileForm from "./Profile/ResumeProfile";
import UserCard from "./Profile/UserCard";

export default {
  components: {
    EditProfileForm,
    UserCard,
  },
  data() {
    return {
      user: {
        fullName: "Amine ITJI",
        title: "Master 1 Informatique",
        description: `À la recherche de nouvelles expériences pour mettre mes compétences en action. Compétent en C++, Java, Python et JavaScript. Maîtrise de Maven, Django et Vue.js. Habileté avancée avec un terminal Linux. Familier avec la méthode Agile et GitHub. Capacité d'adaptation et d'écoute.`,
        contact: {
          phone: "+33 7 82 29 36 20",
          email: "amineitji@gmail.com",
          linkedin: "https://www.linkedin.com/in/amine-itji-5a8696268/",
          github: "https://github.com/amineitji",
          googlePlus: "https://plus.google.com/your-profile-url"
        }
      },
    };
  },
};
</script>

<style>
/* Add any styles here if needed */
</style>
