<script>
	import Link from './Link.svelte';
	import github from '$lib/images/github-mark-white.svg';
	import discord from '$lib/images/discord-mark-blue.svg';
	import deezer from '$lib/images/deezer-mark.svg';
	import profilePic from '$lib/images/profile_picture.png';
</script>

<head>
	<title>AnOliveBranch - Home</title>
</head>

<div id="top">
	<h1>AnOliveBranch</h1>
	<img src={profilePic} alt="Profile" />
	<p>they/she<sup><a href="https://en.pronouns.page/@AnOliveBranch" target="_blank">?</a></sup></p>
</div>

<h2>My Links</h2>

<ul>
	<li>
		<Link img={github} link="https://github.com/AnOliveBranch" title="GitHub" />
	</li>
	<li>
		<Link img={discord} link="https://discord.gg/BgZBg3hBDV" title="Discord" />
	</li>
	<li>
		<Link img={deezer} link="https://www.deezer.com/us/profile/4872646322" title="Deezer" />
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
		flex-wrap: wrap;
	}

	li {
		margin: 2em;
	}

	img {
		width: 150px;
		margin: auto;
		border-radius: 50%;
		border: 5px solid black;
	}

	h1,
	p {
		margin: 0;
	}

	sup a {
		color: rgb(100, 166, 241);
		text-decoration: none;
	}
</style>
