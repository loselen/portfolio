<script lang="ts">
	let { children, class: className = '' } = $props();
</script>

<div class="flex w-full justify-center {className}">
	{@render children()}
</div>
