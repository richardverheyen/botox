<script context="module">
	// @ts-ignore
	export const load = async ({ fetch }) => {
		const res = await fetch('https://api.spacexdata.com/v3/rockets');
		const rockets = await res.json();
		return {
			props: {
				rockets
			}
		};
	};
</script>

<script>
	import Calendar from '$lib/Calendar.svelte';
	  /**
	   * @type {any}
	   */
	 export let rockets = [];
</script>

<svelte:head>
	<title>Home</title>
</svelte:head>

<div class="gutters">
	<h1>Botox</h1>
	<h2>Availabilities</h2>
	<Calendar rockets={rockets} />
</div>

<style lang="scss">
	div.gutters {
		display: flex;
		flex-direction: column;
		min-height: inherit;
	}
</style>
