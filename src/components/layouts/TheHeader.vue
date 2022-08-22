<script>
export default {
  props: ["title"],
};
</script>

<template>
  <header>
    <h1>
      {{ title }}
    </h1>
  </header>
</template>

<style scoped>
header {
  width: 100%;
  height: 5rem;
  background-color: var(--color-background-soft);
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
