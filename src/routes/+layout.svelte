<script lang="ts">
	import { page } from '$app/stores';
	import Header from '$lib/components/Header.svelte';
	import Navbar from '$lib/components/Navbar.svelte';
	import '../app.pcss';
</script>

<Navbar />
<Header title={$page.route.id} />
<main class="mx-auto max-w-7xl py-6 px-4 sm:px-6 lg:px-8">
	<slot />
</main>

<style lang="postcss">
	:global(body) {
		background-color: theme(colors.zinc.900);
		color: theme(colors.zinc.100);
	}
</style>
