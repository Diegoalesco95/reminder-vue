<script>
import StoredResources from './components/learning-resources/StoredResources.vue';
import TheHeader from './components/layouts/TheHeader.vue';

export default {
	components: { StoredResources, TheHeader },
	data() {
		return {
			storedResources: [
				{
					id: 'official-guide',
					title: 'Official Guide',
					description: 'The official vuejs documentation',
					link: 'https://vuejs.org/',
				},
				{
					id: 'google',
					title: 'Google',
					description: 'Search for resources',
					link: 'https://www.google.com',
				},
			],
		};
	},
};
</script>

<template>
	<the-header title="Reminder"></the-header>
	<main>
		<stored-resources :resources="storedResources"></stored-resources>
	</main>
</template>

<style scoped></style>
