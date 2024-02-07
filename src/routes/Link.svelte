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
		<p>{title}</p>
		<img src={img} alt={title} />
		<a href={link} target="_blank">Link</a>
		<button on:click={showBack}>About</button>
	</div>
{:else}
	<div id="back">
		<p>{title}</p>
		<p id="details">{details}</p>
		<button on:click={showFront}>Back</button>
	</div>
{/if}

<style>
	div {
		display: flex;
		flex-direction: column;
		justify-content: center;
		width: 200px;
		border: solid rgb(100, 166, 241) 2px;
	}

	img {
		border-bottom: solid rgb(100, 166, 241) 2px;
		padding: 1em;
		height: 150px;
		object-fit: contain;
	}

	a {
		text-decoration: none;
		color: white;
		text-align: center;
		padding: 0.5em;
		font-size: 1.5em;
		transition: 0.5s;
	}

	a:hover {
		background-color: rgb(120, 186, 255);
	}
</style>
