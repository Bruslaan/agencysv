<script>
	import Card from './Card.svelte';
</script>

<section id="whatwedo" class="max-w-6xl mx-auto min-h-screen p-7 ">
	<h1 class="text-4xl md:text-6xl   font-bold ">What we do for living</h1>
	<p class="text-2xl md:text-4xl text-gray-400 font-light">
		We build software everybody loves to use.
	</p>

	<div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-5 justify-between mt-20">
		<Card title="Ux Design 💅" image="design.png" />
		<Card title="Web Development 💻" image="webdev.png" />
		<Card title="Mobile Development 📲" image="mobiledev.png" />
	</div>

	<div class=" max-w-3xl  mx-auto mt-20">
		<p class="text-center w-full text-2xl md:text-4xl font-serif italic">
			"We adapt to your needs. It’s as minimal or as powerful as you need it to be."
		</p>
	</div>
</section>
