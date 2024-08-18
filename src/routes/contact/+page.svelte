<script>
	import Link from '../Link.svelte';
	import discord from '$lib/images/discord-mark-blue.svg';
	import discordDetails from '$lib/link-details/discord.txt?raw';
	import email from '$lib/images/email-logo.svg';
	import emailDetails from '$lib/link-details/email.txt?raw';
</script>

<head>
	<title>AnOliveBranch - Contact</title>
</head>

<div id="top">
	<h1>Contact Me</h1>
	<p>Need support? Have suggestions? Just want to chat?</p>
</div>

<h2>Contact Options</h2>

<ul>
	<li>
		<Link
			img={discord}
			link="https://discord.gg/BgZBg3hBDV"
			title="Discord"
			details={discordDetails}
		/>
	</li>
	<li>
		<Link img={email} link="mailto:liv@anolivebranch.dev" title="Email" details={emailDetails} />
	</li>
</ul>

<style>
	h1 {
		padding-bottom: 0.5em;
	}

	ul {
		list-style: none;
		display: flex;
		width: 60%;
		margin: auto;
		justify-content: space-around;
		padding: 0;
		flex-wrap: wrap;
	}

	li {
		margin: 2em;
	}

	h1,
	p {
		margin: 0;
	}
</style>
