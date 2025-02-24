<script>
	// src/routes/+page.svelte
	import { source } from 'sveltekit-sse';
	const value = source('/custom-event').select('message');
</script>

{$value}
