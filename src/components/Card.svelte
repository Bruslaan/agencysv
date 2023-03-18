<script>
	export let title;
	export let image = null;
	export let description =
		'We design with love and passion Create your own labels, tags, owners, and more, so everyone has context and everything stays organized.';
</script>

<div class="rounded-lg px-5 pt-5 customgray w-full flex flex-col justify-between min-h-[400px]">
	<div>
		<h1 class="text-2xl font-bold">{title}</h1>

		<p class="mt-5">{description}</p>

		<a class="text-blue-700 -ml-2" href="/">Read more ></a>
	</div>

	{#if image}
		<div class=" overflow-hidden mx-auto  max-w-[80%]">
			<img class="object-fit object-contain max-h-[300px] mix-blend-darken" src={image} alt="" />
		</div>
	{/if}
</div>
