<script>
    //#count
    let count = 0;

    let alertMsg = 0;
    // reactive ($: ngubah check reactive nggaknya secara otomatis)
    $: doubled = count * 2;

    // reactive (another way)
    $: if (count >= 10) {
		alert(`count is dangerously high!`);
        count = 9;
        alertMsg = 1;

        // document.getElementById("myName").style.display = "block"; // ini kalau via hardcode show/hide element by Id
    }
    
    //#count
	function handleClick() {
        count += 1; // count = count + 1;
    }
    //#count
	function resetCount() {
        count = 0;
        alertMsg = 0;
	}
</script>

<h4>3.2 Reactive</h4>
<p>Count: {count}</p>
<p>{count} doubled is {doubled}</p>

<button on:click={handleClick}>
    <!-- ternary condition (true/false condition)   >>    {conditional === a ? true : false} -->
	Clicked {count} {count === 1 ? 'time' : 'times'}
</button>
<button on:click={resetCount} disabled={count >= 1 ? '' : 'disabled'}>
	Reset
</button>

<div id="myName" class="{alertMsg === 1 ? 'alert' : 'd-none'}">count is dangerously high!</div>

<style>
    .d-none {
        display: none;
    }
    .alert {
        background: #ff3e00;
        color: #ffffff;
        padding: 10px;
    }
</style>