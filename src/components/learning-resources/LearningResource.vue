<script>
export default {
  props: { id: String, description: String, link: String, title: String },
};
</script>

<template>
  <li>
    <base-card>
      <header>
        <h3>{{ title }}</h3>
        <button>Delete</button>
      </header>
      <p>{{ description }}</p>
      <nav>
        <a :href="link">View Resource</a>
      </nav>
    </base-card>
  </li>
</template>

<style scoped>
li {
  margin: auto;
  max-width: 40rem;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

h3 {
  font-size: 1.25rem;
  margin: 0.5rem 0;
}

p {
  margin: 0.5rem 0;
}
</style>
