<script>
	let inputString;
</script>

<div class="text-column tool">
	<h1>Dec to Everything converter</h1>
	<p>Input your number here :</p>
	<input bind:value={inputString} />
	<h2>HEX</h2>
	<p>{parseInt(inputString).toString(16)}</p>
	<h2>BIN</h2>
	<p>{parseInt(inputString).toString(2)}</p>
</div>

<style>
	.tool {
		max-width: 40%;
	}
	h1 {
		font-size: 3em;
		font-weight: bold;
	}
	h2 {
		font-size: 2em;
		font-weight: bold;
	}
	input {
		font-size: 1.5em;
	}
</style>
