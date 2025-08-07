<script lang="ts">

	import favicon from '$lib/assets/favicon.svg';
	import Header from '../components/header.svelte';
	import Footer from '../components/footer.svelte';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<div class="min-h-screen flex flex-col selection:bg-(--secondary) selection:text-(--background-color) py-4">
	<Header/>
	<div id="app" class="flex-grow place-items-center">
		<main class="
			px-10
			sm:px-30
			md:px-50
			lg:px-70
			xl:px-90
			2xl:px-120"
		>
			<div class="
			flex
			flex-col
			justify-self-start
			gap-10
			max-w-2xl
			justify-self-center
			">
				{@render children?.()}
			</div>
		</main>
	</div>
	<Footer/>
</div>
