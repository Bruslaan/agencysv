<script>
	import Card from './Card.svelte';
	let y = 0;
	let element;
	let currentIndex = 0;
	let children;
	const exampleContent = [
		{
			title: 'Test Card 1',
			image: 'https://picsum.photos/200/301',
			step: '1. Create a new design'
		},
		{
			title: 'Test Card 2',
			image: 'https://picsum.photos/200/302',
			step: '2. Functional requirements'
		},
		{
			title: 'Test Card 3',
			image: 'https://picsum.photos/200/303',
			step: '3. Technical requirements'
		},
		{
			title: 'Test Card 4',
			image: 'https://picsum.photos/200/304',
			step: '4. Development'
		},
		{
			title: 'Test Card 5',
			image: 'https://picsum.photos/200/305',
			step: '5. Quality assurance'
		},
		{
			title: 'Test Card 6',
			image: 'https://picsum.photos/200/306',
			step: '6. Deployment'
		},
		{
			title: 'Test Card 7',
			image: 'https://picsum.photos/200/306',
			step: '7. Maintenance and updates'
		}
	];
	const setActive = (y) => {
		if (!children) return;
		for (var i = 0; i < children.length; i++) {
			var element = children[i];
			if (element.offsetTop + element.offsetHeight - window.innerHeight / 2 < y) {
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

	$: {
		setActive(y);
	}

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
			class="md:w-1/2  h-[200vh] flex flex-col justify-between  text-4xl font-bold pt-[50%] pb-[50%]"
		>
			{#each exampleContent as content, i}
				<h1 class={currentIndex == i ? 'text-gray-900' : 'text-gray-300'}>{content.step}</h1>
			{/each}
		</div>

		<div
			class="md:w-1/2 sticky md:top-0  bottom-[10%]  md:h-screen flex justify-center items-center"
		>
			<div class="">
				<Card title={exampleContent[currentIndex].title} />
			</div>
		</div>
	</div>
</section>

<svelte:window bind:scrollY={y} />
