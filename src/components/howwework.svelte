<script>
	import Card from './Card.svelte';
	let scrollPosition = 0;
	let element;
	let currentIndex = 0;
	let children;
	const exampleContent = [
		{
			title: 'Test Card 1',
			image: 'https://picsum.photos/200/301',
			step: 'Create a new design'
		},
		{
			title: 'Test Card 2',
			image: 'https://picsum.photos/200/302',
			step: 'Functional requirements'
		},
		{
			title: 'Test Card 3',
			image: 'https://picsum.photos/200/303',
			step: 'Technical requirements'
		},
		{
			title: 'Test Card 4',
			image: 'https://picsum.photos/200/304',
			step: 'Development'
		},
		{
			title: 'Test Card 5',
			image: 'https://picsum.photos/200/305',
			step: 'Quality assurance'
		},
		{
			title: 'Test Card 6',
			image: 'https://picsum.photos/200/306',
			step: 'Deployment'
		},
		{
			title: 'Test Card 7',
			image: 'https://picsum.photos/200/306',
			step: 'Maintenance and updates'
		}
	];
	const setActive = (_scrollPosition) => {
		if (!children) return;
		for (var i = 0; i < children.length; i++) {
			const element = children[i];
			const distanceFromTop = element.offsetTop + element.offsetHeight - window.innerHeight / 2;
			if (distanceFromTop < _scrollPosition) {
				if (currentIndex < i) {
					currentIndex = i;
				}
			} else {
				if (currentIndex > i) {
					currentIndex = i;
				}
			}
		}
	};

	$: setActive(scrollPosition);
	$: children = element?.children;
</script>

<section id="howwework" class="max-w-6xl mx-auto min-h-screen p-7">
	<h1 class="text-4xl md:text-6xl font-bold ">How we work</h1>
	<p class="text-2xl md:text-4xl text-gray-400 font-light">
		We build software everybody loves to use.
	</p>

	<div class="md:flex gap-5">
		<div
			bind:this={element}
			id="track"
			class="md:w-1/3 h-[2000px] flex flex-col justify-between  text-2xl font-bold pt-[50%] pb-[50%]"
		>
			{#each exampleContent as content, i}
				<h1 class={currentIndex == i ? 'text-gray-900' : 'text-gray-300'}>
					<span>{i}.</span>
					{content.step}
				</h1>
			{/each}
		</div>

		<div
			class="md:w-2/3 sticky md:top-0  bottom-[10%]  md:h-screen flex justify-center items-center"
		>
			<div class="">
				<Card title={exampleContent[currentIndex].title} />
			</div>
		</div>
	</div>
</section>

<svelte:window bind:scrollY={scrollPosition} />
