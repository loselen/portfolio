<script lang="ts">
	import { Container } from '$lib/components/container';
	import { Button } from 'bits-ui';
</script>

<Container.Root class="bg-linear-to-b from-zinc-950 to-zinc-900">
	<Container.Content class="md:w-full md:text-2xl">
		<div
			class="-m-4 flex min-h-svh flex-col justify-center gap-4 p-8 md:flex-row md:items-end md:justify-between md:p-12"
		>
			<div class="flex flex-col gap-4">
				<h1 class="text-4xl md:text-7xl">
					Hello,<br class="hidden md:block" /> I am<br class="md:hidden" />
					<strong class="text-orange-500">Loselen</strong>
				</h1>
				<p class="text-zinc-400">
					And this is my personal portfolio.<br class="hidden md:block" /> Currently, there is my learning
					documentation here.
				</p>
			</div>
			<Button.Root
				class="w-fit rounded-md bg-orange-500 px-4 py-2 text-center font-semibold md:px-8"
				href="/docs"
			>
				See my docs
			</Button.Root>
		</div>
	</Container.Content>
</Container.Root>

<Container.Root>
	<Container.Content class="md:w-full md:text-2xl">
		<div class="-m-4 flex min-h-svh flex-col justify-center gap-8 p-8 md:p-12">
			<h2 class="text-2xl md:text-4xl">You can reach me on these platforms</h2>
			<div class="flex flex-col gap-4">
				<a href="mailto:keranairhujan1234@gmail.com">
					<span class="text-orange-500">Email</span> keranairhujan1234@gmail.com
				</a>
				<a href="https://github.com/loselen" target="_blank" rel="noopener noreferrer"
					><span class="text-orange-500">GitHub</span> loselen</a
				>
				<a href="https://instagram.com/loselen.luari" target="_blank" rel="noopener noreferrer">
					<span class="text-orange-500">Instagram</span> loselen.luari
				</a>
			</div>
		</div>
	</Container.Content>
</Container.Root>
