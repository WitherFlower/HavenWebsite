<script>
	let inputString = "";

	function countWords(s) {
		s = s.replace(/(^\s*)|(\s*$)/gi, ""); //exclude  start and end white-space
		s = s.replace(/[ ]{2,}/gi, " "); //2 or more space to 1
		s = s.replace(/\n /, "\n"); // exclude newline with a start spacing
		return s.split(" ").filter(function (str) {
			return str != "";
		}).length;
		//return s.split(' ').filter(String).length; - this can also be used
	}
</script>

<div class="text-column tool">
	<h1>Word Counter</h1>
	<p>Input your text here :</p>
	<input bind:value={inputString} />
	<h2>Words</h2>
	<p>{countWords(inputString)}</p>
	<h2>Characters</h2>
	<p>{inputString.length}</p>
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
