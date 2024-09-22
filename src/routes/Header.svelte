<script>
	import { page } from "$app/stores";
	import logo from "$lib/images/svelte-logo.svg";
	import github from "$lib/images/github.svg";
</script>

<header>
	<nav>
		<ul>
			<li aria-current={$page.url.pathname === "/" ? "page" : undefined}>
				<a href="/">Home</a>
			</li>
			<li
				aria-current={$page.url.pathname === "/tools"
					? "page"
					: undefined}
			>
				<a href="/tools">Tools</a>
			</li>
		</ul>
	</nav>
	<div class="toprightstuff">
		<a class="toprightcontent" href="/lunatic.html">Lunatic Mode</a>
	</div>
</header>

<style>
	header {
		display: flex;
		justify-content: space-around;
		border-bottom-width: 0.15em;
		border-bottom-style: solid;
		border-bottom-color: black;
	}

	.toprightstuff {
		display: flex;
		position: absolute;
		margin: auto;
		height: 3em;
		right: 1em;
		flex: 1;
		flex-direction: row-reverse;
	}

	.toprightcontent {
		margin: auto;
	}

	nav {
		display: flex;
		justify-content: center;
		margin: auto;
	}

	ul {
		position: relative;
		padding: 0;
		margin: 0;
		height: 3em;
		display: flex;
		justify-content: center;
		align-items: center;
		list-style: none;
		background: var(--background);
		background-size: contain;
	}

	li {
		position: relative;
		height: 100%;
	}

	nav a {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 0.5rem;
		color: var(--color-text);
		font-weight: 700;
		font-size: 0.8rem;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		text-decoration: none;
		transition: color 0.2s linear;
	}

	a:hover {
		color: var(--color-theme-1);
	}
</style>
