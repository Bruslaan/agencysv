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

<slot />
