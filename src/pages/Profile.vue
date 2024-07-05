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
import EditProfileForm from "./Profile/EditProfileForm";
import UserCard from "./Profile/UserCard";

export default {
  components: {
    EditProfileForm,
    UserCard,
  },
  data() {
    return {
      model: {
        company: "Creative Code Inc.",
        email: "amineitji@gmail.com",
        username: "amineitji",
        firstName: "Amine",
        lastName: "ITJI",
        address: "Lyon / Paris",
        city: "Lyon",
        country: "France",
        about:
          "",
      },
      user: {
        fullName: "Amine ITJI",
        title: "Étudiant en Master 1 Informatique",
        description: `À la recherche de nouvelles experiences pour mettre mes compétences en action. Compétent en C++, Java, Python et Javascript. Maîtrise de Maven, Django et Vue.js. Habileté avancée avec un terminal Linux. Familier à la méthode Agile et à GitHub. Capacité d'adaptation et d'écoute.`,
        contact: {
          phone: "+33 7 82 29 36 20",
          email: "amineitji@gmail.com",
          linkedin: "https://www.linkedin.com/in/amine-itji-5a8696268/",
          github: "https://github.com/amineitji"
        }
      },
    };
  },
};
</script>

<style>
/* Add any styles here if needed */
</style>
