<script lang="ts">
	import Footer from '$lib/components/footer/Footer.svelte';
	import '../app.postcss';
	import Header from '$lib/components/header/Header.svelte';

	export let data;
</script>

<div class="app">
	<Header shopName={data.config?.shopName} />

	<main class="container mx-auto">
		<slot />
	</main>

	<Footer serverTime={data.serverDate} />
</div>
