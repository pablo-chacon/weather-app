<template>
  <button class="search-btn" @click="handleButton">{{ text }}</button>
</template>

<script>
import { defineComponent } from "vue";
export default defineComponent({
  name: "ButtonSearch",
  props: {
    text: String,
  },
  methods: {
    handleButton() {
      this.$emit("customMethod");
    },
  },
});
</script>

<style scoped>
.search-btn {
  width: 100%;
  font-size: 26px;
  padding: 0.25em 1em;
  margin-bottom: 1em;
}
</style>
