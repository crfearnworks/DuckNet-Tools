<script>
	import Navbar from "./Navbar.svelte";
	import ToolLink from "./ToolLink.svelte";
	import Footer from "./Footer.svelte";

	let tools = [
		{
			name: "Svelte",
			description: "A new way to build web applications.",
			url: "https://svelte.dev"
		},
		{
			name: "Sapper",
			description: "The next small thing in web development.",
			url: "https://sapper.svelte.dev"
		}
	];

</script>

<Navbar />

<div class="container">
	{#each tools as tool}
		<ToolLink name={tool.name} description={tool.description} url={tool.url} />
	{/each}
</div>

<Footer />

<style>
	.container {
		max-width: 800px;
		margin: 0 auto;
		padding: 2rem;
	}
</style>