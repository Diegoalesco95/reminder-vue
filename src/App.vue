<script>
import TheHeader from "./components/layouts/TheHeader.vue";
import TheResources from "./components/learning-resources/TheResources.vue";

export default {
  components: { TheHeader, TheResources },
};
</script>

<template>
  <the-header title="Reminder"></the-header>
  <main>
    <the-resources></the-resources>
  </main>
</template>

<style scoped></style>
