<script>
	import db from "$lib/db";
</script>

<div>
	<h1>Leaderboard</h1>
	<table>
		<thead>
			<tr>
				<th>WA</th>
				<th>Partners</th>
			</tr>
		</thead>
		<tbody>
			{#each db.WAs.sort((a, b) => b.partners - a.partners) as WA}
				<tr>
					<td>{WA.name}</td>
					<td>{WA.partners}</td>
				</tr>
			{/each}
		</tbody>
	</table>
	<!-- {#each db.WAs.sort((a, b) => b.partners - a.partners) as WA}
		<p>{WA.name} - {WA.partners}</p>
	{/each} -->
</div>

<style>
	div {
		border: #333 solid 1px;
		border-radius: 10px;
		padding: 10px;
		margin: 10px;
		background: #f0f0f0;
		color: #333;
	}
</style>
