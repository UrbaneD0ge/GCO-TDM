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
				<tr key={WA.name} class="leaderboard-row">
					<!-- <td>
						<img src={WA.logo} alt={WA.name} width="50" height="50" />
					</td> -->
					<td>{WA.name}</td>
					<td>{WA.partners}</td>
				</tr>
			{/each}
		</tbody>
	</table>
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

	td:nth-child(2) {
		padding: 10px;
		text-align: center;
	}

	.leaderboard-row {
		cursor: pointer;
		border-radius: 20px;
	}

	.leaderboard-row:hover {
		background-color: #e0e0e0;
		transition: background-color 0.3s ease;
	}
</style>
