<script>
	import Link from './Link.svelte';
	import github from '$lib/images/github-mark-white.svg';
	import discord from '$lib/images/discord-mark-blue.svg';
</script>

<head>
	<title>AnOliveBranch - Home</title>
</head>

<ul>
	<li>
		<Link img={github} link="https://github.com/AnOliveBranch" title="GitHub" />
	</li>
	<li>
		<Link img={discord} link="https://discord.gg/BgZBg3hBDV" title="Discord" />
	</li>
	<li>
		<Link img={github} link="https://github.com/AnOliveBranch" title="GitHub" />
	</li>
	<li>
		<Link img={github} link="https://github.com/AnOliveBranch" title="GitHub" />
	</li>
	<li>
		<Link img={github} link="https://github.com/AnOliveBranch" title="GitHub" />
	</li>
</ul>

<style>
	ul {
		list-style: none;
		display: flex;
		justify-content: space-around;
		padding: 0;
	}
</style>
