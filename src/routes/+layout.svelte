<script>
	import '../app.css';
	import { onMount } from 'svelte';
	onMount(() => {
		import('../cursor');
	});
</script>

<svelte:head>
	<script src="https://cdn.jsdelivr.net/npm/particles.js@2.0.0/particles.min.js"></script>
</svelte:head>

<div class="sticky top-0 z-50">
	<div id="cursor" class="cursor z-50">
		<div class="cursor__content" />
	</div>
</div>

<div class="flex justify-center items-center  text-white pt-12">
	<img src="logo.white2.png" class="w-40" alt="" />
</div>

<div class="inset-0 absolute -z-30" id="particles-js">
	<img
		src="background.JPG"
		class="bg-cover object-cover h-full w-full absolute inset-0 -z-30"
		alt=""
	/>
</div>

<div
	class="uppercase text-white flex gap-6 justify-center text-center font-thin fixed bottom-0 right-0 left-0 p-8"
>
	<!-- footer -->
	<a class="" href="/">Home</a>
	<a href="/">KNOWLEDGE HUB</a>
	<a href="/about">Imprint</a>
</div>

<slot />
