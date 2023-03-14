<script lang="ts">
	import { hideFareZones } from '../../routes/stores';
</script>

<div class="main">
	<h2>Map options</h2>
	<input
		type="checkbox"
		name="hide-fare-zones"
		id="hide-fare-zones"
		bind:checked={$hideFareZones}
	/>
	<label for="hide-fare-zones">Hide fare zones</label>
</div>

<style>
	.main {
		padding: 10px;
		height: 80px;
		border-bottom: 1px solid #3c3c3c;
		height: 100%;
	}
</style>
