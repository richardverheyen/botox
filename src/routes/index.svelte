<svelte:head>
  <title>Home</title>
</svelte:head>

<script>
	import Calendar from '$lib/Calendar.svelte';
</script>

<div class="gutters">
    <h1>Botox</h1>
    <h2>Availabilities</h2>
    <Calendar />
</div>

<style lang="scss">
	div.gutters {
        display: flex;
        flex-direction: column;
        min-height: inherit;
    }
</style>