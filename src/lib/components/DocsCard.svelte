<script lang="ts">
	type Tag = {
		name: string;
		color: string;
	};

	let {
		title,
		description,
		date,
		tags
	}: {
		title: string;
		description: string;
		date: string;
		tags: Tag[];
	} = $props();
</script>

<div class="flex flex-col rounded-lg border border-zinc-500">
	<div class="h-32 w-full rounded-t-lg outline outline-zinc-500 md:h-40"></div>
	<div class="flex flex-col gap-3 p-4">
		<div class="flex w-full flex-row flex-wrap gap-1">
			{#each tags as tag (tag.name)}
				<p class="w-fit rounded-full px-2 text-xs" style="background-color: {tag.color};">
					#{tag.name}
				</p>
			{/each}
		</div>
		<div class="flex flex-col gap-1">
			<h2 class="text-base leading-5 font-semibold md:text-lg">{title}</h2>
			<p class="text-xs text-zinc-400 md:text-sm">{date}</p>
		</div>
		<p class="text-zinc-300">{description}</p>
	</div>
</div>
