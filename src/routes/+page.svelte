<script>
	import Map from '$lib/components/Map.svelte';
	import Sidebar from '$lib/components/Sidebar.svelte';
	import TopBar from '$lib/components/TopBar.svelte';
</script>

<svelte:head>
	<title>MTR Map View</title>
	<meta name="description" content="Map of my MTR world in Minecraft" />
</svelte:head>

<section>
	<div class="over">
		<div />
	</div>
	<TopBar />

	<div class="sidebyside">
		<Sidebar />
		<Map />
	</div>
</section>

<style>
	.sidebyside {
		display: flex;
		align-items: flex-start;
	}

	.over {
		position: absolute;
		z-index: 10;
	}
</style>
