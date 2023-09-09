<template>
  <div class="input-form">
    <label class="input-label"> {{ label }} </label>
    <v-text-field
      v-model="model"
      class="input-search"
      placeholder="Búsqueda"
      prepend-inner-icon="mdi-magnify"
      :type="type"
      dense
      outlined
      hide-details
    >
    </v-text-field>
  </div>
</template>

<script>
export default {
  name: "BaseSearch",
  props: {
    label: { type: String, default: "" },
    placeholder: { type: String, default: "" },
    type: { type: String, default: "text" },
    value: { type: String, default: "" },
  },
  computed: {
    model: {
      get() {
        return this.value;
      },
      set(value) {
        this.$emit("input", value);
      },
    },
  },
  data: () => ({}),
};
</script>
