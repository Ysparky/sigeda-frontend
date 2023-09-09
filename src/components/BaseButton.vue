<template>
  <v-btn
    class="my-3 pa-5"
    depressed
    flat
    rounded
    style="
      color: #ffffff;
      background: #6f51ff;
      margin: auto;
      text-transform: capitalize;
      font-weight: 600;
    "
    @click="$emit('click', $event)"
  >
    {{ name }}
  </v-btn>
</template>

<script>
export default {
  name: "BaseButton",
  props: {
    name: { type: String, default: "" },
  },
};
</script>
