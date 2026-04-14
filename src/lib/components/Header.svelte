<script>
	import arrowLeft from '$lib/images/arrow-left.svg';
	let { skip = false } = $props();
</script>

<div class="header items-center p-4">
	<img src={arrowLeft} alt="" />
	<p class="grow text-center text-xl font-semibold">Business Name</p>
	{#if skip}
		<p class="text-gray-400">Skip</p>
	{/if}
</div>

<style>
	.header {
		display: flex;
		justify-content: space-between;
	}
</style>
