<script>
	import Card from './Card.svelte';
	let y = 0;
	let element;
	let currentIndex = 0;
	const exampleContent = [
		{
			title: 'Test Card 1',
			image: 'https://picsum.photos/200/301'
		},
		{
			title: 'Test Card 2',
			image: 'https://picsum.photos/200/302'
		},
		{
			title: 'Test Card 3',
			image: 'https://picsum.photos/200/303'
		},
		{
			title: 'Test Card 4',
			image: 'https://picsum.photos/200/304'
		},
		{
			title: 'Test Card 5',
			image: 'https://picsum.photos/200/305'
		},
		{
			title: 'Test Card 6',
			image: 'https://picsum.photos/200/306'
		},
		{
			title: 'Test Card 7',
			image: 'https://picsum.photos/200/306'
		}
	];
	let audio;
	const setActive = (y, element) => {
		if (!element) return;
		const children = element.children;

		for (var i = 0; i < children.length; i++) {
			var element = children[i];
			// Do stuff
			if (element.offsetTop + element.offsetHeight - window.innerHeight / 2 < y) {
				element.classList.add('text-gray-900');
				currentIndex = i;
			} else {
				element.classList.remove('text-gray-900');
			}
		}
	};

	$: {
		setActive(y, element);
	}
</script>

<section id="howwework" class="max-w-6xl mx-auto min-h-screen p-7">
	<h1 class="text-4xl md:text-6xl font-bold ">How we work</h1>
	<p class="text-2xl md:text-4xl text-gray-400 font-light">
		We build software everybody loves to use.
	</p>

	<audio bind:this={audio} id="beep" src="https://amie.so/audio/scrollwheel.mp3" />
	<div class="md:flex gap-5">
		<div
			bind:this={element}
			id="track"
			class="md:w-1/2  h-[200vh] flex flex-col justify-between  text-4xl font-bold pt-[50%] pb-[50%]"
		>
			<h1 class="text-gray-300">Create a new design for the User experience</h1>
			<h1 class="text-gray-300">Functional requirements</h1>
			<h1 class="text-gray-300">Technical requirements</h1>
			<h1 class="text-gray-300">Development</h1>
			<h1 class="text-gray-300">Quality assurance</h1>
			<h1 class="text-gray-300">Deployment</h1>
			<h1 class="text-gray-300">Maintenance and updates</h1>
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
