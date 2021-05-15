<script>
	export let item;
	export let i = '';
	export let lang = 'fi-FI';
	let options = {
		year: 'numeric',
		month: '2-digit',
		day: '2-digit',
		hour: '2-digit',
		minute: '2-digit',
	};
	if (i == 1) options.weekday = 'short';
	let date = new Date(item).toLocaleDateString(lang, options);
	date = !i ? date.split(' ')[0] : date.replaceAll(' klo ', ' ');
</script>

{date}
