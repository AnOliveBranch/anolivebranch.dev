<script>
	import transflag from '$lib/images/trans-flag.svg';
	import mle from '$lib/images/logo-mle-256.png';
	import profilePic from '$lib/images/selfie.jpg';
</script>

<head>
	<title>AnOliveBranch - About</title>
</head>

<div id="top">
	<h1>About Me - Liv</h1>
	<img src={profilePic} alt="Profile" id="pfp" />
</div>

<ul>
	<li>
		<h2>Queer to the core</h2>
		<p>I am an agender transfemme polyamorous lesbian</p>
		<img src={transflag} alt="Transgender pride flag" />
		<p>
			I am loud and proud when it comes to my queer identity. I openly talk about my experiences,
			and seek to make others feel welcome in expressing their true selves. My queerness is an
			integral part of me, I won't brush it to the side.
		</p>
	</li>
	<li>
		<h2>Professional Developer</h2>
		<p>
			I work full time as a security automation engineer in the insurance industry. I'm passionate
			about my work and building process improvements wherever I can.
		</p>
	</li>
	<li>
		<h2>Community Leader</h2>
		<img src={mle} alt="MLE logo" />
		<p>
			I hold the position of board member and director of community for Minor League Esports. My
			positions come with many responsibilities as one of the most visible high-level staff members
			in the community.
		</p>
	</li>
	<li>
		<h3>Board Member</h3>
		<p>
			As an MLE board member, I work on high level organization and planning for the league. I work
			with the league financials and managing the structure and goals of the organization as a
			whole.
		</p>
		<h3>Community Director</h3>
		<p>
			As the MLE director of community, I oversee admissions, events, moderation, and user
			experience for the entire league. I drive change any place I can to improve the departments
			under me. I work with the department coordinators to ensure they have the necessary tools to
			run their departments.
		</p>
	</li>
</ul>

<style>
	h1,
	h2,
	p,
	img {
		padding-bottom: 0.5em;
	}

	ul {
		list-style: none;
		display: flex;
		width: 80%;
		margin: auto;
		justify-content: space-around;
		padding: 0;
		flex-wrap: wrap;
	}

	li {
		margin: 2em;
		width: 20%;
	}

	h1,
	p {
		margin: 0;
	}

	img {
		display: block;
		margin: auto;
		border-radius: 5%;
	}

	#pfp {
		padding: 0;
		height: 150px;
		width: 150px;
		margin: auto;
		border-radius: 50%;
		border: 5px solid rgb(100, 166, 241);
	}
</style>
