<script>
	import { page } from '$app/stores';
	import triangle from '$lib/images/triangle.svg';
</script>

<header>
	<nav>
		<ul>
			<li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
				<a href="/">
					Home
					<img src={triangle} alt="Current Page" />
				</a>
			</li>
			<li aria-current={$page.url.pathname === '/projects' ? 'page' : undefined}>
				<a href="/projects">
					Projects
					<img src={triangle} alt="Current Page" />
				</a>
			</li>
			<li aria-current={$page.url.pathname === '/about' ? 'page' : undefined}>
				<a href="/about">
					About
					<img src={triangle} alt="Current Page" />
				</a>
			</li>
			<li aria-current={$page.url.pathname === '/contact' ? 'page' : undefined}>
				<a href="/contact">
					Contact
					<img src={triangle} alt="Current Page" />
				</a>
			</li>
		</ul>
	</nav>
</header>

<style>
	nav {
		text-align: center;
		border-bottom: 2px solid rgb(100, 166, 241);
		position: relative;
	}

	ul {
		display: flex;
		justify-content: space-around;
		align-items: stretch;
		margin: 0;
		padding: 0;
	}

	ul li {
		display: flex;
		padding: 0;
		font-size: 1.5em;
		position: relative;
		flex: 1;
	}

	li a {
		color: white;
		text-decoration: none;
		padding: 1em 0;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		width: 100%;
		box-sizing: border-box;
		transition: 0.5s;
	}

	li img {
		display: none;
		position: absolute;
		bottom: 0;
		left: 50%;
		transform: translateX(-50%);
		width: 20px;
		height: auto;
	}

	li[aria-current='page'] img {
		display: block;
	}

	li a:hover {
		background-color: rgb(120, 186, 255);
	}
</style>