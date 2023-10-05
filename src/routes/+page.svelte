<script>
	import { onMount } from 'svelte';

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

		const submitFormAnchor = document.getElementById('mc-embedded-subscribe-button');
		const myForm = document.getElementById('mc-embedded-subscribe-form');

		submitFormAnchor.addEventListener('click', function (event) {
			event.preventDefault(); // Prevent the default behavior (navigation)
			// Trigger form submission
			myForm.submit();
		});
	});

	

</script>

<title>Tadm Nutrition</title>

<div />

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
			<form
				action="https://tadm-nutrition.us9.list-manage.com/subscribe/post?u=fbd221b20ed4da0c283581efc&amp;id=4b16948ce9&amp;f_id=005914e1f0"
				method="post"
				id="mc-embedded-subscribe-form"
				name="mc-embedded-subscribe-form"
				class="validate"
				target="_blank"
			>
				<input
					
					type="email"
					name="EMAIL"
					id="mce-EMAIL"
					required=""
					value=""
					placeholder="Your email here"
					class="rounded-lg h-10 px-4 bg-transparent w-full font-thin italic  text-white"
				/>
				<a
					type="submit"
					name="subscribe"
					id="mc-embedded-subscribe-button"
					class="absolute right-0 top-0 bottom-0 pr-8 uppercase text-white">Subscribe</a
				>
			</form>
		</div>
	</div>
</div>
