<script>
	import Map from '$lib/components/Map.svelte';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<div class="over">
		<div />
	</div>

	<Map />
</section>

<style>
	.over {
		position: absolute;
		z-index: 10;
	}
</style>
