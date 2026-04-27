<script lang="ts">
	let { children, class: className = ""} = $props();
</script>

<div class="w-full flex justify-center">
	<div class="w-xl p-4 {className}">
		{@render children()}
	</div>
</div>
