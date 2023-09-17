<svelte:head>
	<title>How to play Sverdle | Legible</title>
	<meta name="description" content="How to play Sverdle" />
</svelte:head>

<div class="text-column">
	<h2>How to play Sverdle</h2>

	<p>
		Sverdle is a clone of <a href="https://www.nytimes.com/games/wordle/index.html">Wordle</a>, the
		word guessing game. To play, enter a five-letter English word. For example:
	</p>

	<div class="example">
		<span class="letter close">r</span>
		<span class="letter missing">i</span>
		<span class="letter close">t</span>
		<span class="letter missing">z</span>
		<span class="letter exact">y</span>
	</div>

	<p>
		The <kbd class="exact">y</kbd> is in the right place. <kbd class="close">r</kbd> and
		<kbd class="close">t</kbd>
		are the right letters, but in the wrong place. The other letters are wrong, and can be discarded.
		Let's make another guess:
	</p>

	<div class="example">
		<span class="letter exact">p</span>
		<span class="letter exact">a</span>
		<span class="letter exact">r</span>
		<span class="letter exact">t</span>
		<span class="letter exact">y</span>
	</div>

	<p>This time we guessed right! You have <strong>six</strong> guesses to get the word.</p>

	<p>
		Unlike the original Wordle, Sverdle runs on the server instead of in the browser, making it
		impossible to cheat. It uses <code>&lt;form&gt;</code> and cookies to submit data, meaning you can
		even play with JavaScript disabled!
	</p>
</div>

<style>
	span {
		display: inline-flex;
		justify-content: center;
		align-items: center;
		font-size: 0.8em;
		width: 2.4em;
		height: 2.4em;
		box-sizing: border-box;
		border-radius: 2px;
		border-width: 2px;
	}
	
	.example {
		display: flex;
		justify-content: flex-start;
		margin: 1rem 0;
		gap: 0.2rem;
	}

	.example span {
		font-size: 1.4rem;
	}

	p span {
		position: relative;
		border-width: 1px;
		border-radius: 1px;
		font-size: 0.4em;
		transform: scale(2) translate(0, -10%);
		margin: 0 1em;
	}
</style>
