<script>
	import quotes from '$lib/data/collection.json';
</script>

<div class="flex bg-white">
	<div class="flex-none w-1/6 p-4 pt-12">
		<h1 class="text-left pl-6 text-3xl text-black font-bold">Quips</h1>
		<h2 class="text-left pt-2 pl-6 text-xl text-black">This code is on fire</h2>
	</div>
	<div class="flex-initial w-3/6 center">
		<div class="grid grid-cols-3 gap-2 p-4 max-w-6xl pl-12 pt-12">
			{#each quotes as quip}
				<div class="w-full h-0 shadow-md pb-full border-solid border border-slate-400 bg-slate-50">
					<span
						class="inline-block align-text-bottom font-serif p-6 leading-8 text-md whitespace-pre-wrap"
						>{quip}</span
					>
				</div>
			{/each}
		</div>
	</div>
</div>

<!-- <p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p> -->

<!-- <h1 class="text-3xl font-bold underline">Hello world!</h1> -->

<style lang="postcss">
	:global(html) {
		background-color: theme(colors.gray.100);
	}
</style>
