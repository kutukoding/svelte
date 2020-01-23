<script>
	// ambil name dari main.js
	export let name
	import Training3 from './3_event.svelte'
	import Training32 from './3_event_advance.svelte'
</script>

<main>
	<h1><span class="blue"></span>Hello {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>

	<!-- event (click) -->
	<hr/>
	<Training3/>
	<Training32/>
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