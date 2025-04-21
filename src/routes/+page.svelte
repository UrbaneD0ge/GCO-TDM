<script>
	import Leaderboard from "../components/Leaderboard.svelte";
	import Progress from "../components/Progress.svelte";
</script>

<svelte:head>
	<title>GCO Dashboard</title>
	<meta name="description" content="GCO Dashboard for Contract Year 3" />
	<link rel="icon" href="/favicon.png" />
	<meta name="viewport" content="width=device-width, initial-scale=1.0" />
	<meta name="theme-color" content="#ffffff" />
	<meta property="og:title" content="GCO Dashboard" />
	<meta property="og:description" content="GCO Dashboard for Contract Year 3" />
</svelte:head>

<div>
	<h1>GCO Dashboard</h1>
	<p>Welcome to GCO Contract Year 3! Check your progress below!</p>
</div>

<section>
	<Progress />
	<Leaderboard />
</section>

<style>
	section {
		display: flex;
		width: 100%;
	}
	* {
		font-family: Arial, sans-serif;
	}

	:global(body) {
		font-family: Arial, Helvetica, sans-serif;
	}
	div {
		margin: 10;
		padding: 50;
		/* background: #f0f0f0; */
	}
</style>
