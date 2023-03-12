<script>
	import '../app.css';
	import { onMount } from 'svelte';

	onMount(() => {
		import('../cursor');
	});
</script>

<div class="sticky top-0 z-50">
	<div id="cursor" class="cursor z-50">
		<div class="cursor__content" />
	</div>
</div>

<slot />
