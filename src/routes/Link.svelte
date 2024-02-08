<script>
	export let img = '';
	export let link = '';
	export let title = '';
	export let details = 'Some details';

	let side = 'front';

	function showBack() {
		side = 'back';
	}

	function showFront() {
		side = 'front';
	}
</script>

{#if side == 'front'}
	<div id="front">
		<p id="title">{title}</p>
		<img src={img} alt={title} />
		<div class="bottom">
			<a href={link} target="_blank">Link</a>
			<button on:click={showBack}>About</button>
		</div>
	</div>
{:else}
	<div id="back">
		<p id="title">{title}</p>
		<p id="details">{details}</p>
		<button class="bottom" on:click={showFront}>Back</button>
	</div>
{/if}

<style>
	div#front,
	div#back {
		display: flex;
		flex-direction: column;
		justify-content: space-around;
		width: 200px;
		height: 300px;
		background-color: rgb(40, 40, 40);
		border-radius: 10%;
		box-shadow: -3px 3px 5px 10px rgb(35, 35, 35);
	}

	div#front:hover,
	div#back:hover {
		border: 2px solid rgb(100, 166, 241);
	}

	img,
	p#details {
		padding: 0 1em 1em 1em;
		margin: 0;
		height: 150px;
		object-fit: contain;
	}

	p,
	a,
	button {
		font-family: Georgia, 'Times New Roman', Times, serif;
		text-align: center;
	}

	a {
		text-decoration: none;
		color: white;
		text-align: center;
		font-size: 1.5em;
		transition: 0.5s;
		margin: 0;
		padding: 0;
	}

	button {
		border: none;
		background: none;
		color: white;
		font-size: 1.5em;
		cursor: pointer;
		margin: 0;
		padding: 0;
	}

	.bottom {
		display: flex;
		justify-content: space-around;
	}

	.bottom a,
	.bottom button,
	button.bottom {
		padding: 1em;
	}

	p#title {
		margin: 0;
		font-size: 1.5em;
	}
</style>
