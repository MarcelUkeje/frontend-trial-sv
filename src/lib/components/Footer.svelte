<script>
	import NavigationLink from './NavigationLink.svelte';
	let { href, textContent = 'Continue' } = $props();
</script>

<div class="flex flex-col items-center py-4">
	<NavigationLink {href} {textContent} />
</div>
