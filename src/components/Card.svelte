<script>
	export let title;
	export let image = null;
</script>

<div class="rounded-lg px-5 pt-5 customgray w-full flex flex-col justify-between min-h-[400px]">
	<div>
		<h1 class="text-2xl font-bold">{title}</h1>

		<p class="mt-5">
			We design with love and passion Create your own labels, tags, owners, and more, so everyone
			has context and everything stays organized.
		</p>
	</div>

	{#if image}
		<img class="max-h-56 bg-contain" src={image} alt="" />
	{/if}
</div>
