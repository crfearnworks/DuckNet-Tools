<script>
	import { onMount } from "svelte";	
	import Navbar from "../../lib/Navbar.svelte";
	import ToolLink from "../../lib/ToolLink.svelte";
	import Footer from "../../lib/Footer.svelte";

	let tools = [];

	onMount(async () => {
		const response = await fetch("/tools.json");
		tools = await response.json();
	});

</script>

<Navbar />

<div class="container">
	{#each tools as tool}
		<ToolLink {tool} />
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