<template>
  <div class="d-flex fill-height justify-center align-center bg-login">
    <v-card
      class="elevation-3 d-flex flex-column"
      style="background: #f8f7fb; padding: 4em 3em"
    >
      <v-img
        style="margin: auto; margin-bottom: 3em"
        max-height="200"
        max-width="200"
        src="../assets/images/logo-empresa.png"
      ></v-img>
      <base-input label="Código" placeholder="Código de alumno" />
      <base-input label="Contraseña" placeholder="*************" />
      <v-btn
        class="my-3 pa-5"
        depressed
        flat
        rounded
        style="color: #ffffff; background: #2f80ed; margin: auto"
      >
        Ingresar
      </v-btn>
    </v-card>
  </div>
</template>

<script>
import BaseInput from "@/components/BaseInput.vue";
export default {
  components: {
    BaseInput,
  },
  name: "LoginView",
};
</script>

<style lang="scss" scoped>
.bg-login {
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
    url("../assets/images/bg-fpe.png");
  background-position: 50% 0;
  background-size: cover;
}
</style>
