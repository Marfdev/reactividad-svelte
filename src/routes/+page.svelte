<script>
	let count = 0;

	function handleClick() {
		count += 1;
	}

    $: evenOrOdd = count % 2 === 0 ? 'even' : 'odd';
</script>

<button on:click={handleClick}>
	Clicked {count}
	{count === 1 ? 'time' : 'times'}
</button>
<span>
    count is {evenOrOdd}
</span>
