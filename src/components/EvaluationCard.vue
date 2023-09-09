<template>
  <div class="card-container">
    <v-container>
      <v-row class="align-center" no-gutters>
        <v-col cols="6" class="card-title">Contacto 1</v-col>
        <v-col cols="6" class="card-type text-end">Adaptación</v-col>
        <v-col cols="12" class="card-text pl-3">Evaluador: Tomas Ortiz</v-col>
        <v-col cols="12" class="card-text pl-3 pb-2">Fecha: 16-01-2023</v-col>
        <v-col cols="12" class="card-subtitle">Evaluación</v-col>
        <v-col cols="4" class="card-text">Diego Falconi</v-col>
        <v-col cols="4" class="card-text text-center">☆ 14.61</v-col>
        <v-col cols="4" class="card-text text-end" style="color: #21b454"
          >Vuelo Bueno</v-col
        >
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "EvaluationCard",
};
</script>

<style lang="scss" scoped>
.card-container {
  background-color: rgba(47, 127, 237, 0.2);
  border-radius: 1em !important;
  width: 23em;
}

.card {
  font-style: normal;
  line-height: normal;

  &-title {
    font-size: 1.5rem;
    font-weight: 600;
  }

  &-type {
    font-size: 1.25rem;
    font-weight: 400;
    color: #ed3237;
  }

  &-text {
    font-size: 1rem;
    font-weight: 400;
  }

  &-subtitle {
    font-size: 1rem;
    font-weight: 600;
  }
}
</style>
