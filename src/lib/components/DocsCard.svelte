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

<div class="flex gap-3 rounded-lg border border-zinc-500 p-3">
	<div class="flex flex-col gap-3">
		<div class="h-24 w-32 rounded-lg border border-zinc-500"></div>
		<div class="flex w-32 flex-row flex-wrap gap-1">
			{#each tags as tag (tag.name)}
				<p class="w-fit rounded-full px-2 text-xs" style="background-color: {tag.color};">
					#{tag.name}
				</p>
			{/each}
		</div>
	</div>
	<div class="flex flex-col gap-2">
		<div class="flex flex-col gap-1">
			<h2 class="text-base leading-5 font-semibold">{title}</h2>
			<p class="text-xs text-zinc-400">{date}</p>
		</div>
		<p>{description}</p>
	</div>
</div>
