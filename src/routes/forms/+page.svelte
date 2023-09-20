<svelte:head>
	<title>Forms | Legible</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<div class="text-column">
	<h2>Forms</h2>
	<form style="display: flex; flex-direction: column; gap: 8px;">
		<div>
			<select>
				<option></option>
				<option>HELLO</option>
				<option>WORLD</option>
			</select>
		</div>
		<div>
			<input>
		</div>
		<div>
			<textarea></textarea>
		</div>
		<div>
			<button type="submit">Do It</button>
		</div>
	</form>
</div>
