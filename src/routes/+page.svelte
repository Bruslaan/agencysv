<script>
	import { onMount } from "svelte";

	// import Navbar from '../components/navbar.svelte';
	// import Header from '../components/header-tadm.svelte';
	// import Hero from '../components/hero.svelte';
	// import Howwework from '../components/howwework.svelte';
	// import Showcase from '../components/showcase.svelte';
	// import Stackingcards from '../components/stackingcards.svelte';
	// import Footer from '../components/footer.svelte';
	// import Faq from '../components/accordion.svelte';

	

	onMount(() => {
		particlesJS.load('particles-js', 'particles.json', function () {
		console.log('callback - particles.js config loaded');
	});
	});

</script>

<title>Tadm Nutrition</title>


<div>

</div>

<!-- Header -->
<div class="flex justify-center items-center  text-white pt-12 ">
	<img src="logo.white.svg" class="" alt="" />
</div>

<div class="flex flex-col text-center justify-center items-center h-[70vh]">
	<div class="flex flex-col justify-between h-[40vh] ">
		<div>
			<h1 class="text-8xl text-white text-center font-semibold">Coming Soon</h1>
			<br />
			<p class="text-white w-[70%] mx-auto">
				We are just a few weeks away from a big launch. Sign up to be notified!
			</p>
		</div>

		<div class="relative w-[70%] mx-auto">
			<div class="bg-white opacity-30 w-full absolute inset-0 -z-10 rounded-lg" />
			<input
				placeholder="Your email here"
				class="rounded-lg h-10 px-4 bg-transparent w-full font-thin italic  text-white"
				type="text"
			/>
			<a href="/" class="absolute right-0 top-0 bottom-0 pr-8 uppercase text-white">Subscribe</a>
		</div>
	</div>
</div>

<div

	class="uppercase text-white flex gap-6 justify-center text-center font-thin fixed bottom-0 right-0 left-0 p-8"
>
	<!-- footer -->
	<a class="" href="/">Imprint</a>
	<a href="/">KNOWLEDGE HUB</a>
	<a href="/">CONTACT</a>
</div>

<div class="inset-0 absolute -z-30" id="particles-js">
	<img
		src="background.JPG"
		class="bg-cover object-cover h-full w-full absolute inset-0 -z-30"
		alt=""
	/>
</div>

<!-- <Navbar />
<Hero /> -->

<!-- <Faq /> -->
<!-- <Footer /> -->

<!-- <Stackingcards /> -->
