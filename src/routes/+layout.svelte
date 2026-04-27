<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	import Container from '../components/Container.svelte';
	import '@fontsource-variable/elms-sans/wght.css';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>

<div class="min-h-svh bg-zinc-900 text-zinc-100 font-elms">
	<Container>
		{@render children()}
	</Container>
</div>

<style>
	.font-elms {
		font-family: 'Elms Sans Variable', sans-serif;
	}
</style>