<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<h1>WitherFlower's Backyard (or something)</h1>

<section>
	<img
		class="counter"
		src="https://count.pek.li/get/@:WitherWebsite?theme=gelbooru"
		alt=":VisitCounter"
	/>
</section>

<style>
	h1 {
		font-weight: bold;
		font-size: 3em;
	}
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}
</style>
