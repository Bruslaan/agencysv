<script>
	import Statistics from './Statistics.svelte';

	import Card from './Card.svelte';
</script>

<section id="whatwedo" class="max-w-6xl mx-auto min-h-screen p-7 ">
	<h1 class="text-4xl md:text-6xl   font-bold ">Take a look what we did</h1>
	<p class="text-2xl md:text-4xl text-gray-400 font-light">
		We build software everybody loves to use.
	</p>

	<Statistics />

	<div class="grid md:grid-cols-3 gap-5 mt-20">
		<div class="md:col-span-2">
			<Card
				title="Droov.io"
				image="https://www.notion.so/cdn-cgi/image/format=auto,width=750,quality=100/front-static/pages/home/meeting-notes.png"
				description="We design with love and passion Create your own labels, tags, owners, and more, so everyone has context and everything stays organized."
			/>
		</div>

		<Card
			title="Paarfit"
			image="https://www.notion.so/cdn-cgi/image/format=auto,width=750,quality=100/front-static/pages/home/meeting-notes.png"
			description="lorem	ipsum"
		/>
		<Card
			title="Reinio.io"
			image="https://www.notion.so/cdn-cgi/image/format=auto,width=750,quality=100/front-static/pages/home/meeting-notes.png"
			description="Visualize, filter & sort any way you want
			Show only tasks assigned to you, or items marked as urgent. Break down any project in the way that’s most helpful to you.
			Visualize, filter & sort any way you wa"
		/>
		<div class="md:col-span-2">
			<Card
				title="Sometest.io"
				image="https://www.notion.so/cdn-cgi/image/format=auto,width=750,quality=100/front-static/pages/home/meeting-notes.png"
			/>
		</div>
	</div>
</section>
