<script>
export default {
  props: ["mode"],
};
</script>

<template>
  <button :class="mode">
    <slot></slot>
  </button>
</template>

<style scoped>
button {
  padding: 0.75rem 1.5rem;
  font-family: inherit;
  background-color: var(--primary);
  border: var(--primary);
  color: white;
  cursor: pointer;
}

button:hover,
button:active {
  background-color: var(--primary);
  border: var(--primary);
}

.flat {
  background-color: transparent;
  color: var(--primary);
  border: none;
}

.flat:hover,
.flat:active {
  background-color: var(--color-background-soft);
  color: var(--color-text);
}
</style>
