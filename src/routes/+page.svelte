<script>
	import Map from '$lib/components/Map.svelte';
</script>

<svelte:head>
	<title>MTR Map View</title>
	<meta name="description" content="Map of my MTR world in Minecraft" />
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
