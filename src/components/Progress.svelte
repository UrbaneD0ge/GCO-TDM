<script>
	import db from "$lib/db";
	let progress = 30;
</script>

<div>
	<h1>Progress</h1>

	<!-- Progress Meter goes here -->
	<div id="progress"></div>
</div>

<style>
	:root {
		--progress: 30%;
	}

	div {
		border: #333 solid 1px;
		border-radius: 10px;
		padding: 10px;
		margin: 10px;
		background: #f0f0f0;
		color: #333;
	}

	#progress {
		background: #333;
		border-radius: 13px;
		height: 20px;
		width: 300px;
		padding: 3px;
	}

	#progress:after {
		content: "";
		display: block;
		background: orange;
		width: var(--progress);
		height: 100%;
		border-radius: 9px;
	}
</style>
