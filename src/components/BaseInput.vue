<template>
  <div class="input-form">
    <label class="input-label"> {{ label }} :</label>
    <v-text-field
      v-model="model"
      class="input-text"
      :type="type"
      :placeholder="placeholder"
      dense
      flat
      outlined
    />
  </div>
</template>

<script>
export default {
  name: "BaseInput",
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
