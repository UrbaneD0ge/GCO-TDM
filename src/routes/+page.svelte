<script>
	import Leaderboard from "../components/Leaderboard.svelte";
	import Progress from "../components/Progress.svelte";
</script>

<div>
	<h1>GCO Dashboard</h1>
	<p>Welcome to GCO Contract Year 3! Check your progress below!</p>
</div>

<Progress />
<Leaderboard />

<style>
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
