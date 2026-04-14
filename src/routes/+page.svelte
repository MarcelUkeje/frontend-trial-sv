<svelte:head>
	<title>Home</title>
</svelte:head>

<div class="mx-0 flex flex-row justify-center gap-1 border bg-cyan-200 px-6 py-2">
	<h1 class="text-lg font-bold text-blue-500 text-shadow-lg">Tailwind CSS</h1>
</div>
<div class="main">
	<div
		class="main-content text-mono flex flex-col items-stretch justify-center gap-1 border p-1 [&_a]:text-center [&_a]:font-bold [&_a]:text-red-700"
	>
		<a class="items-start border text-start font-mono" href="/forty">Fortieth Screen</a>
		<a class="items-start border text-start font-mono" href="/forty-one">Forty-First Screen</a>
		<a class="items-start border text-start font-mono" href="/forty-two">Forty-Second Screen</a>
		<!-- <p>Remember to add a 'Back to homepage button'</p> -->
	</div>
</div>

<style>
	.main-content a:nth-child(2n + 1) {
		background-color: #00c950;
	}
	.main-content a:nth-child(2n) {
		background-color: #ff6900;
	}
</style>
