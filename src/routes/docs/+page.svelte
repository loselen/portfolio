<script lang="ts">
	import { resolve } from '$app/paths';
	import { Container } from '$lib/components/container';
	import DocsCard from '$lib/components/DocsCard.svelte';
	import { ArrowLeft } from '@lucide/svelte';
</script>

<Container.Root>
	<Container.Content class="flex flex-col gap-8 py-16 text-sm">
		<div class="flex items-center gap-2">
			<a href={resolve('/')}>
				<ArrowLeft size={32} />
			</a>
			<h1 class="text-2xl">Learning Docs</h1>
		</div>
		<div class="flex flex-col gap-3">
			<DocsCard
				title="VGG vs MLP on CIFAR-10: A Comparative Study"
				description="Exploring the performance gap between a simple multi-layer perceptron and a deep convolutional network on the CIFAR-10 benchmark. Covers training setup, accuracy curves, and overfitting behavior."
				date="27 Apr 2026"
				tags={[
					{ name: 'deep-learning', color: '#7C3AED' },
					{ name: 'computer-vision', color: '#0EA5E9' }
				]}
			/>
			<DocsCard
				title="Understanding Backpropagation from Scratch"
				description="A step-by-step walkthrough of the backpropagation algorithm using only NumPy. Derives gradients manually for a 2-layer network and verifies them with finite differences."
				date="24 Apr 2026"
				tags={[
					{ name: 'math', color: '#D97706' },
					{ name: 'deep-learning', color: '#7C3AED' }
				]}
			/>
			<DocsCard
				title="Attention Is All You Need — Paper Notes"
				description="Personal reading notes on the original Transformer paper. Breaks down multi-head self-attention, positional encoding, and why the architecture replaced RNNs for sequence modeling."
				date="20 Apr 2026"
				tags={[
					{ name: 'nlp', color: '#059669' },
					{ name: 'paper-review', color: '#6B7280' }
				]}
			/>
			<DocsCard
				title="Setting Up a PyTorch Training Loop"
				description="A minimal but complete training loop in PyTorch with gradient clipping, learning rate scheduling, and checkpoint saving. Designed as a reusable template for future experiments."
				date="15 Apr 2026"
				tags={[
					{ name: 'pytorch', color: '#EF4444' },
					{ name: 'deep-learning', color: '#7C3AED' }
				]}
			/>
		</div>
	</Container.Content>
</Container.Root>
