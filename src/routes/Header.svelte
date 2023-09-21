<script>
	import { page } from '$app/stores';
	import logo from '$lib/images/svelte-logo.svg';
	import github from '$lib/images/github.svg';
</script>

<header>
	<h1>Legible</h1>
	<!-- TODO: Search? -->
	<!-- TODO: Collapse menu on mobile -->
	<nav>
		<ul>
			<li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
				<a href="/">Home</a>
			</li>
			<li aria-current={$page.url.pathname === '/about' ? 'page' : undefined}>
				<a href="/about">About</a>
			</li>
			<li aria-current={$page.url.pathname === '/forms' ? 'page' : undefined}>
				<a href="/forms">Forms</a>
			</li>
			<li aria-current={$page.url.pathname.startsWith('/sverdle') ? 'page' : undefined}>
				<a href="/sverdle">Sverdle</a>
			</li>
		</ul>
	</nav>
</header>

<!-- TODO: Move to app.css -->
<style>
	header {
		display: flex;
		max-width: var(--column-width);
		width: calc(100% - 32px);
		flex-direction: column;
		justify-content: flex-start;
		margin: 8px 16px;
	}

	ul {
		position: relative;
		padding: 0;
		margin: 0;
		height: 2rem;
		display: flex;
		gap: 8px;
		list-style: none;
		background: var(--background);
		background-size: contain;
	}

	li {
		position: relative;
		height: 100%;
	}

	li[aria-current='page'] {
		border-bottom: 4px solid var(--color-highlight);
		margin-bottom: -4px;
	}

	nav a {
		display: flex;
		height: 100%;
		align-items: center;
		color: var(--color-text);
		font-weight: 700;
		font-size: 0.8rem;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		text-decoration: none;
		transition: color 0.2s linear;
	}

	a:hover {
		color: var(--color-highlight);
	}
</style>
