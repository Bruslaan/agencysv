<script>
	import AccordionItem from './accordionItem.svelte';
	const data = [
		{
			question: 'What is Svelte?',
			answer: 'Svelte is a compiler for building'
		},
		{
			question: 'How does Svelte work?',
			answer: 'Svelte is a compiler for building'
		},
		{
			question: "What's the difference between Svelte and React?",
			answer: 'Svelte is a compiler for building'
		},
		{
			question: "What's the difference between Svelte and Vue?",
			answer: 'Svelte is a compiler for building'
		},
		{
			question: "What's the difference between Svelte and Angular?",
			answer: 'Svelte is a compiler for building'
		}
	];
</script>

<section id="faq" class="max-w-6xl mx-auto min-h-screen p-7  mt-20">
	<h1 class="text-4xl md:text-6xl font-bold text-center">Any Questions?</h1>

	<div class="mt-20">
		{#each data as entry}
			<AccordionItem {entry} />
		{/each}
	</div>
</section>
