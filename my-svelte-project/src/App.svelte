<script>
	// ambil name dari main.js
	export let name

	import Training1 from './1_nested.svelte'
</script>

<main>
	<h1><span class="blue"></span>Hello {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
	
	<!-- nested components (termasuk @html komponen) -->
	<hr/>
	<Training1/>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>