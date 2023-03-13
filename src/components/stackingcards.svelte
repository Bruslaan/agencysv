<section id="stackingcards" class="max-w-6xl mx-auto min-h-screen p-7 ">
	<h1 class="text-4xl md:text-6xl   font-bold ">What we do for living</h1>
	<p class="text-2xl md:text-4xl text-gray-400 font-light">
		We build software everybody loves to use.
	</p>

	<div class="wrapper mt-20">
		<div class="scroll-cards mt-20">
			<article class="scroll-cards__item rounded-lg px-5 pt-5 customgray" aria-label="Wie - 1">
				<h2>Nice little headline</h2>
			</article>
			<article class="scroll-cards__item" aria-label="Wie - 1">
				<h2>Nice little headline</h2>
			</article>
			<article class="scroll-cards__item" aria-label="Wie - 1">
				<h2>Nice little headline</h2>
			</article>
			<article class="scroll-cards__item" aria-label="Wie - 1">
				<h2>Nice little headline</h2>
			</article>
			<article class="scroll-cards__item" aria-label="Wie - 1">
				<h2>Nice little headline</h2>
			</article>
		</div>
	</div>
</section>

<style>
	.wrapper {
		max-width: 60em;
		margin: 0 auto;
	}

	.scroll-cards {
		counter-reset: card;
		position: relative;
		display: block;
		padding-bottom: 120vh;
	}

	.scroll-cards > .scroll-cards__item + .scroll-cards__item {
		margin-top: 40vh;
	}

	.scroll-cards__item {
		--offset: 0.5em;
		color: #000;
		position: sticky;
		top: max(16vh, 10em);
		padding: 2em 1.5em;
		min-height: 19em;
		background: #fff;
		box-shadow: 0 2px 40px rgba(0, 0, 0, 0.1);
		width: calc(100% - 5 * var(--offset));
	}

	.scroll-cards__item:nth-of-type(0) {
		transform: translate(calc((0 - 1) * var(--offset)), calc((0 - 1) * var(--offset)));
	}
	.scroll-cards__item:nth-of-type(1) {
		transform: translate(calc((1 - 1) * var(--offset)), calc((1 - 1) * var(--offset)));
	}
	.scroll-cards__item:nth-of-type(2) {
		transform: translate(calc((2 - 1) * var(--offset)), calc((2 - 1) * var(--offset)));
	}
	.scroll-cards__item:nth-of-type(3) {
		transform: translate(calc((3 - 1) * var(--offset)), calc((3 - 1) * var(--offset)));
	}
	.scroll-cards__item:nth-of-type(4) {
		transform: translate(calc((4 - 1) * var(--offset)), calc((4 - 1) * var(--offset)));
	}
	.scroll-cards__item:nth-of-type(5) {
		transform: translate(calc((5 - 1) * var(--offset)), calc((5 - 1) * var(--offset)));
	}
</style>
