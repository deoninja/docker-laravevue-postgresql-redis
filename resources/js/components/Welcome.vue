<template>
    <h1>Deo Docker laravel + postgresql</h1>
  Hello {{ name }} welcome to my app.
  <hr />
  <counter></counter>
</template>
<script lang="ts">
import { defineComponent, ref } from "vue";
import Counter from "./Counter.vue";

export default defineComponent({
  components: {
    Counter,
  },
  setup() {
    const name = ref<string>("Everyone");
    return {
      name,
    };
  },
});
</script>
