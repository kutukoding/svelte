<script>
    let count = 0;
    
	function handleClick() {
        count += 1; // count = count + 1;
    }
	function resetCount() {
        count = 0;
	}
</script>

<h2>step-3: event & reactivity</h2>

<h4>3.1 Event on Click</h4>
<p>Count: {count}</p>

<button on:click={handleClick}>
	Clicked {count}x
</button>
<button on:click={resetCount}>
	Reset
</button>