<script>
	import { slide } from 'svelte/transition';
	export let entry;
	let isOpen = false;
	const toggle = () => (isOpen = !isOpen);
</script>

<div class="border-b max-w-3xl m-auto">
	<button
		class="flex justify-between w-full py-5 text-gray-800 cursor-none"
		on:click={toggle}
		aria-expanded={isOpen}
	>
		<h1 class="text-2xl text-left">{entry.question}</h1>
		<svg
			style="tran"
			width="20"
			height="20"
			fill="none"
			stroke-linecap="round"
			stroke-linejoin="round"
			stroke-width="2"
			viewBox="0 0 24 24"
			stroke="currentColor"><path d="M9 5l7 7-7 7" /></svg
		>
	</button>
	{#if isOpen}
		<div class="mt-5 text-gray-500 mb-5 text-xl font-light">
			<p transition:slide={{ duration: 200 }}>
				{entry.answer}
			</p>
		</div>
	{/if}
</div>

<style>
	svg {
		transition: transform 0.2s ease-in;
	}

	[aria-expanded='true'] svg {
		transform: rotate(0.25turn);
	}
</style>
