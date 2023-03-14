<script lang="ts">
	import {
		l1Active,
		l2Active,
		l3Active,
		l4Active,
		l5Active,
		m1Active,
		m2Active,
		m3Active,
		allActive
	} from '../../routes/stores';

	function getActiveRouteName() {
		switch (true) {
			case $l1Active:
				return 'L1';
			case $l2Active:
				return 'L2';
			case $l3Active:
				return 'L3';
			case $l4Active:
				return 'L4';
			case $l5Active:
				return 'L5';
			case $m1Active:
				return 'M1';
			case $m2Active:
				return 'M2';
			case $m3Active:
				return 'M3';
		}
	}
</script>

<aside class="main">
	<h2>Line details</h2>

	{#if $allActive}
		<p>Select a line to get started.</p>
	{:else}
		<h3>Line {getActiveRouteName()}</h3>
	{/if}
</aside>

<style>
	aside {
		padding: 10px;
		width: 200px;
		border-right: 1px solid #3c3c3c;
	}
</style>
