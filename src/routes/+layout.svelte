<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	import '@fontsource-variable/elms-sans/wght.css';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>

<div class="font-elms min-h-svh bg-zinc-900 text-zinc-100">
	{@render children()}
</div>

<style>
	.font-elms {
		font-family: 'Elms Sans Variable', sans-serif;
	}
</style>
