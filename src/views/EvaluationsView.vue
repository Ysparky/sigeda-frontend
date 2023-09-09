<template>
  <div
    class="d-flex flex-column fill-height justify-center align-center"
    style="background-color: #f8f7fb; padding: 2em 5em"
  >
    <div
      class="d-flex flex-column"
      style="height: 20vh; width: 100%; padding: 2em; gap: 2em"
    >
      <span class="body-title mr-auto">Evaluaciones</span>
      <div class="d-flex flex-row" style="width: inherit; gap: 1em">
        <base-button name="Nuevo Turno" />
        <base-button name="Nuevo Reporte" />
        <v-spacer></v-spacer>
        <base-search></base-search>
      </div>
    </div>
    <v-card
      class="d-flex d-row flex-wrap justify-space-between fill-height pa-6"
      elevation="5"
      style="width: 100%; gap: 1.5em; overflow-y: auto"
      shaped
    >
      <evaluation-card v-for="index in 20" :key="index" />
    </v-card>
  </div>
</template>

<script>
import BaseButton from "@/components/BaseButton.vue";
import BaseSearch from "@/components/BaseSearch.vue";
import EvaluationCard from "@/components/EvaluationCard.vue";

export default {
  name: "EvaluationsView",
  components: { BaseButton, BaseSearch, EvaluationCard },
};
</script>
