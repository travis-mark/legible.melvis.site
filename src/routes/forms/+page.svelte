<svelte:head>
	<title>Forms | Legible</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<div class="text-column">
	<h2>Forms</h2>
	<form style="display: flex; flex-direction: column; gap: 8px;">
		<!-- TODO Labels -->
		<div>
			<!-- TODO Opt group -->
			<select>
				<option></option>
				<option>HELLO</option>
				<option>WORLD</option>
			</select>
		</div>
		<div>
			<!-- TODO Input types -->
			<input>
		</div>
		<div>
			<!-- TODO Default width x height -->
			<textarea></textarea>
		</div>
		<div>
			<!-- TODO Styling -->
			<button type="submit">Do It</button>
		</div>
	</form>
</div>
