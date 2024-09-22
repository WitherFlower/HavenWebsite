<script>
	import Converter from "./Converter.svelte";
	import WordCounter from "./WordCounter.svelte";
</script>

<svelte:head>
	<title>About</title>
	<meta name="description" content="About this app" />
</svelte:head>

<div class="row">
	<Converter />
	<WordCounter />
</div>

<style>
	.row {
		display: flex;
		flex-direction: row;
		width: 100%;
		justify-content: space-between;
	}
</style>
