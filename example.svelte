<script>
	import Datetime from './date.svelte';
	let dates = [
		"2021-05-09 10:37:41",
		"2021-06-21 15:48:21"
	];
</script>

{#each dates as item}
	<Datetime {item} i="1"/>
{/each}
