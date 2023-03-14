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
		allActive,
		hideFareZones
	} from '../../routes/stores';

	function setAll(value: boolean) {
		$m1Active = value;
		$m2Active = value;
		$m3Active = value;
		$l1Active = value;
		$l2Active = value;
		$l3Active = value;
		$l4Active = value;
		$l5Active = value;
		$allActive = value;
	}
</script>

<svg width="100%" viewBox="0 0 3907 2828" fill="none" xmlns="http://www.w3.org/2000/svg">
	<g id="Day Map" clip-path="url(#clip0_425_170)">
		<rect width="3907" height="2828" fill="white" />
		<path id="Background" d="M0 0H3907V2828H0V0Z" fill="#1E1E1E" />
		{#if !$hideFareZones}
			<path
				id="Zone 1 background"
				d="M1748 969.5C1803.23 969.5 1848 924.728 1848 869.5V-8.00001C1848 -63.2285 1892.77 -108 1948 -108H2025C2080.23 -108 2125 -63.2285 2125 -8V378C2125 433.228 2169.77 478 2225 478H2678C2733.23 478 2778 522.772 2778 578V1031.5V1315C2778 1370.23 2733.23 1415 2678 1415H2470.5C2415.27 1415 2370.5 1459.77 2370.5 1515V1776.25C2370.5 1811.46 2399.04 1840 2434.25 1840V1840C2469.46 1840 2498 1868.54 2498 1903.75V2133C2498 2188.23 2453.23 2233 2398 2233H2329C2273.77 2233 2229 2277.77 2229 2333V2431C2229 2486.23 2184.23 2531 2129 2531H1428C1372.77 2531 1328 2575.77 1328 2631V2894.5C1328 2949.73 1283.23 2994.5 1228 2994.5H1202C1146.77 2994.5 1102 2949.73 1102 2894.5V2531V2292.5C1102 2237.27 1146.77 2192.5 1202 2192.5H1432C1487.23 2192.5 1532 2147.73 1532 2092.5V1863C1532 1807.77 1576.77 1763 1632 1763H1748C1803.23 1763 1848 1718.23 1848 1663V1529C1848 1473.77 1803.23 1429 1748 1429H1715.5C1660.27 1429 1615.5 1384.23 1615.5 1329V1069.5C1615.5 1014.27 1660.27 969.5 1715.5 969.5H1748Z"
				fill="#3C3C3C"
			/>
			<path
				id="Zone 3 background"
				d="M3328 922.5V-55C3328 -110.228 3372.77 -155 3428 -155H3509.69H3838C3893.23 -155 3938 -110.228 3938 -55V431V984.5V1368V1793V2186V2906C3938 2961.23 3893.23 3006 3838 3006H3428C3372.77 3006 3328 2961.23 3328 2906V2145.5V1716V1382V922.5Z"
				fill="#3C3C3C"
			/>
		{/if}
		<line
			id="Station connection"
			x1="1335.47"
			y1="1597.68"
			x2="1464.79"
			y2="1521.69"
			stroke="#D9D9D9"
			stroke-width="10"
			stroke-dasharray="10 10"
		/>
		<path
			id="Station connection_2"
			d="M1641 2257L1741 2257"
			stroke="#D9D9D9"
			stroke-width="10"
			stroke-dasharray="10 10"
		/>
		<path
			id="Metro 2"
			on:click={() => {
				if ($allActive) {
					setAll(false);
					$m2Active = true;
				} else {
					setAll(true);
				}
			}}
			class="m2 line"
			class:dim={!$m2Active}
			d="M2243 109V844C2243 899.228 2198.23 944 2143 944H150.5"
			stroke="#1C48E2"
			stroke-width="30"
			stroke-linecap="square"
			stroke-linejoin="round"
		/>
		<path
			id="Metro 1"
			on:click={() => {
				if ($allActive) {
					setAll(false);
					$m1Active = true;
				} else {
					setAll(true);
				}
			}}
			class="m1 line"
			class:dim={!$m1Active}
			d="M1755 2257V1695C1755 1639.77 1710.23 1595 1655 1595H919C863.772 1595 819 1550.23 819 1495V944"
			stroke="#079F4D"
			stroke-width="30"
			stroke-linecap="square"
		/>
		<rect id="Rectangle 32" x="1740" y="1834" width="30" height="83" fill="#3C3C3C" />
		<rect id="Rectangle 33" x="1331" y="1580" width="30" height="30" fill="#1E1E1E" />
		<rect id="Rectangle 34" x="1448" y="929" width="30" height="30" fill="#1E1E1E" />
		<rect id="Rectangle 35" x="1448" y="1506" width="30" height="13" fill="#1E1E1E" />
		<path
			id="Local Trains 4"
			on:click={() => {
				if ($allActive) {
					setAll(false);
					$l4Active = true;
				} else {
					setAll(true);
				}
			}}
			class="l4 line"
			class:dim={!$l4Active}
			d="M1636 2731L1636 2037C1636 1970.73	 1689.73 1917 1756 1917H2268L2815 1917C2892.32 1917 2955 1854.32 2955 1777V1493"
			stroke="#0CA3E3"
			stroke-width="10"
			stroke-linecap="square"
		/>
		<path
			id="Local Trains 4_2"
			on:click={() => {
				if ($allActive) {
					setAll(false);
					$l4Active = true;
				} else {
					setAll(true);
				}
			}}
			class="l4 line"
			class:dim={!$l4Active}
			d="M1616 2731L1616 2037C1616 1959.68 1678.68 1897 1756 1897H2255L2815 1897C2881.27 1897 2935 1843.27 2935 1777V1493.19"
			stroke="#0CA3E3"
			stroke-width="10"
			stroke-linecap="square"
		/>
		<rect
			id="Rectangle 36"
			x="1448"
			y="1610"
			width="30"
			height="59"
			transform="rotate(-90 1448 1610)"
			fill="#1E1E1E"
		/>
		<path
			id="Local Trains 1"
			on:click={() => {
				if ($allActive) {
					setAll(false);
					$l1Active = true;
				} else {
					setAll(true);
				}
			}}
			class="l1 line"
			class:dim={!$l1Active}
			d="M2059 1113V1116C2059 1171.23 2103.77 1216 2159 1216L2765 1216C2825.75 1216 2875 1265.25 2875 1326V1777C2875 1810.14 2848.14 1837 2815 1837L2261.75 1837L1553 1837C1508.82 1837 1473 1801.18 1473 1757L1473 934V795C1473 739.772 1428.23 695 1373 695H1123"
			stroke="#DDB011"
			stroke-width="10"
			stroke-linecap="square"
		/>
		<path
			id="Local Trains 1_2"
			on:click={() => {
				if ($allActive) {
					setAll(false);
					$l1Active = true;
				} else {
					setAll(true);
				}
			}}
			class="l1 line"
			class:dim={!$l1Active}
			d="M2079 1113V1116C2079 1160.18 2114.82 1196 2159 1196L2765 1196C2836.8 1196 2895 1254.2 2895 1326V1777C2895 1821.18 2859.18 1857 2815 1857L2264.25 1857L1553 1857C1497.77 1857 1453 1812.23 1453 1757L1453 934L1450.43 793.539C1449.64 749.933 1414.06 715 1370.45 715H1124"
			stroke="#DDB011"
			stroke-width="10"
			stroke-linecap="square"
		/>
		<path
			id="Local Trains 2a"
			on:click={() => {
				if ($allActive) {
					setAll(false);
					$l2Active = true;
				} else {
					setAll(true);
				}
			}}
			class="l2 line"
			class:dim={!$l2Active}
			d="M1931 1246H2222.86H2765C2809.18 1246 2845 1281.82 2845 1326V1513"
			stroke="#D81159"
			stroke-width="10"
			stroke-linecap="square"
		/>
		<path
			id="Local Trains 2a_2"
			on:click={() => {
				if ($allActive) {
					setAll(false);
					$l2Active = true;
				} else {
					setAll(true);
				}
			}}
			class="l2 line"
			class:dim={!$l2Active}
			d="M2014 1226H2233.33H2765C2820.23 1226 2865 1270.77 2865 1326V1513"
			stroke="#D81159"
			stroke-width="10"
			stroke-linecap="square"
		/>
		<path
			id="Local Trains 3"
			on:click={() => {
				if ($allActive) {
					setAll(false);
					$l3Active = true;
				} else {
					setAll(true);
				}
			}}
			class="l3 line"
			class:dim={!$l3Active}
			d="M1356 1585V1787C1356 1831.18 1391.82 1867 1436 1867H2261.31H2815C2864.71 1867 2905 1826.71 2905 1777V1084C2905 1028.77 2860.23 984 2805 984H1977"
			stroke="#7813A8"
			stroke-width="10"
			stroke-linecap="square"
		/>
		<path
			id="Local Trains 3_2"
			on:click={() => {
				if ($allActive) {
					setAll(false);
					$l3Active = true;
				} else {
					setAll(true);
				}
			}}
			class="l3 line"
			class:dim={!$l3Active}
			d="M1336 1585V1787C1336 1842.23 1380.77 1887 1436 1887H2264.69H2815C2875.75 1887 2925 1837.75 2925 1777V1084C2925 1017.73 2871.27 964 2805 964H1977"
			stroke="#7813A8"
			stroke-width="10"
			stroke-linecap="square"
		/>
		<rect id="Rectangle 37" x="1479" y="1745" width="28" height="164" fill="#1E1E1E" />
		<path
			id="Local Trains 2"
			on:click={() => {
				if ($allActive) {
					setAll(false);
					$l2Active = true;
				} else {
					setAll(true);
				}
			}}
			class="l2 line"
			class:dim={!$l2Active}
			d="M1606 2731V2124.72C1606 2093.12 1580.38 2067.5 1548.78 2067.5V2067.5C1523.5 2067.5 1503 2047 1503 2021.72L1503 1326C1503 1281.82 1538.82 1246 1583 1246H1949C2004.23 1246 2049 1201.23 2049 1146V1118.5V1113"
			stroke="#D81159"
			stroke-width="10"
			stroke-linecap="square"
		/>
		<path
			id="Local Trains 2_2"
			on:click={() => {
				if ($allActive) {
					setAll(false);
					$l2Active = true;
				} else {
					setAll(true);
				}
			}}
			class="l2 line"
			class:dim={!$l2Active}
			d="M1586 2731V2131.63C1586 2106.34 1565.5 2085.85 1540.22 2085.85V2085.85C1508.62 2085.85 1483 2060.23 1483 2028.63L1483 1326C1483 1270.77 1527.77 1226 1583 1226H1949C1993.18 1226 2029 1190.18 2029 1146V1124.5V1113"
			stroke="#D81159"
			stroke-width="10"
			stroke-linecap="square"
		/>
		<text
			id="Pirate Beach"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="475.055" y="1273.55">Pirate Beach</tspan></text
		>
		<text
			id="Spawn Village"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="854" y="1097.55">Spawn Village</tspan></text
		>
		<text
			id="Birch Cape"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="49.375" y="1003.55">Birch Cape</tspan></text
		>
		<text
			id="Cotton Hills Jungle Village"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"
			><tspan x="406.852" y="1003.55">Cotton Hills </tspan><tspan x="385.27" y="1051.55"
				>Jungle Village</tspan
			></text
		>
		<text
			id="Coastal Swamp"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="420.094" y="1449.55">Coastal Swamp</tspan></text
		>
		<text
			id="Birch Mountains"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="1140.09" y="1361.55">Birch Mountains</tspan></text
		>
		<text
			id="Crater Village"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="1184.06" y="1193.55">Crater Village</tspan></text
		>
		<text
			id="Meadow Lake Town"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="1793.92" y="2265.55">Meadow Lake Town&#10;</tspan></text
		>
		<text
			id="Meadow Lake Island"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"
			><tspan x="1178.69" y="2270.55">Meadow Lake Island&#10;</tspan><tspan x="1564" y="2318.55"
				>&#10;</tspan
			></text
		>
		<text
			id="Birch Hill"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="1298.96" y="1996.55">Birch Hill</tspan></text
		>
		<text
			id="Wolf Village"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="1343.34" y="2730.55">Wolf Village</tspan></text
		>
		<text
			id="The Bad Men Mountain"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="1775.95" y="1816.55">The Bad Men Mountain</tspan></text
		>
		<text
			id="Grand Lush Cave"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="998.211" y="1671.55">Grand Lush Cave</tspan></text
		>
		<text
			id="Spruce Village"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="1519" y="1538.55">Spruce Village&#10;</tspan></text
		>
		<text
			id="New Heights Village"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="2068.73" y="1979.55">New Heights Village</tspan></text
		>
		<text
			id="Snowy Mountain Village"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"
			><tspan x="2630.95" y="1967.55">Snowy Mountain </tspan><tspan x="2725.15" y="2015.55"
				>Village</tspan
			></text
		>
		<text
			id="Spruce Basin Village"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"
			><tspan x="2413.39" y="1768.55">Spruce Basin </tspan><tspan x="2474.15" y="1816.55"
				>Village</tspan
			></text
		>
		<text
			id="Cliffside Birch Lake"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="2355.54" y="1311.55">Cliffside Birch Lake</tspan></text
		>
		<text
			id="Lakeside Icy Mountain"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="2401.55" y="1506.55">Lakeside Icy Mountain</tspan></text
		>
		<text
			id="Woodland Mansion"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"
			><tspan x="3116.11" y="1566.55">Woodland </tspan><tspan x="3130.91" y="1614.55">Mansion</tspan
			></text
		>
		<text
			id="Acacia Hill Village Downhill"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"
			><tspan x="3398.69" y="1427.55">Acacia Hill </tspan><tspan x="3348.08" y="1475.55"
				>Village Downhill</tspan
			></text
		>
		<text
			id="Acacia Lake Village"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"
			><tspan x="3669.14" y="1566.55">Acacia Lake </tspan><tspan x="3719.65" y="1614.55"
				>Village</tspan
			></text
		>
		<text
			id="Cliffside Village"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="2104" y="1138.55">Cliffside Village&#10;</tspan></text
		>
		<text
			id="Crazy Mountain"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="1622" y="1200.55">Crazy Mountain&#10;</tspan></text
		>
		<text
			id="Cliffside Village South"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"
			><tspan x="1936.76" y="1311.55">Cliffside Village </tspan><tspan x="2026.88" y="1359.55"
				>South</tspan
			></text
		>
		<text
			id="Abanoned Village"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="1484" y="911.545">Abanoned Village</tspan></text
		>
		<text
			id="Cotton Hills Airport"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="1134" y="679.545">Cotton Hills Airport</tspan></text
		>
		<text
			id="Cotton Hills Lake"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="643" y="445.545">Cotton Hills Lake&#10;</tspan></text
		>
		<text
			id="Cotton Hills Acacia"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"
			><tspan x="627.352" y="805.545">Cotton Hills </tspan><tspan x="673.855" y="853.545"
				>Acacia</tspan
			></text
		>
		<text
			id="Northern Sea Beaches"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"
			><tspan x="1954" y="873.545">Northern Sea </tspan><tspan x="1954" y="921.545">Beaches</tspan
			></text
		>
		<text
			id="Ocean Monument"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="2270" y="806.545">Ocean Monument</tspan></text
		>
		<text
			id="Carved Lake Island"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"
			><tspan x="2270" y="583.545">Carved Lake </tspan><tspan x="2270" y="631.545">Island</tspan
			></text
		>
		<text
			id="Fisherman&#226;&#128;&#153;s Island"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"
			><tspan x="2270" y="359.545">Fisherman&#x2019;s </tspan><tspan x="2270" y="407.545"
				>Island</tspan
			></text
		>
		<text
			id="Blacksmith Village"
			fill="#D9D9D9"
			xml:space="preserve"
			style="white-space: pre"
			font-family="Inter"
			font-size="40"
			letter-spacing="0em"><tspan x="2270" y="123.545">Blacksmith Village</tspan></text
		>
		<g id="M2 box">
			<rect id="Rectangle 7" x="117" y="844" width="70" height="70" rx="20" fill="#1C48E2" />
			<text
				id="M2"
				fill="white"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="36"
				letter-spacing="0em"><tspan x="125.088" y="892.091">M2</tspan></text
			>
		</g>
		<g id="L1 box">
			<rect id="Rectangle 7_2" x="1127" y="732" width="70" height="70" rx="20" fill="#DDB011" />
			<text
				id="L1"
				fill="#1E1E1E"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="36"
				letter-spacing="0em"><tspan x="1144.33" y="780.091">L1</tspan></text
			>
		</g>
		<g id="L3 box">
			<rect id="Rectangle 7_3" x="1884" y="974" width="70" height="70" rx="20" fill="#7813A8" />
			<text
				id="L3"
				fill="white"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="36"
				letter-spacing="0em"><tspan x="1897.41" y="1022.09">L3</tspan></text
			>
		</g>
		<g id="L4 box">
			<rect id="Rectangle 7_4" x="2945" y="1300" width="70" height="70" rx="20" fill="#0CA3E3" />
			<text
				id="L4"
				fill="white"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="36"
				letter-spacing="0em"><tspan x="2958.33" y="1348.09">L4</tspan></text
			>
		</g>
		<g id="L5 box">
			<rect id="Rectangle 7_5" x="2945" y="1398" width="70" height="70" rx="20" fill="#FF8200" />
			<text
				id="L5"
				fill="white"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="36"
				letter-spacing="0em"><tspan x="2958.92" y="1446.09">L5</tspan></text
			>
		</g>
		<g id="L5 box_2">
			<rect id="Rectangle 7_6" x="3761" y="1398" width="70" height="70" rx="20" fill="#FF8200" />
			<text
				id="L5_2"
				fill="white"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="36"
				letter-spacing="0em"><tspan x="3774.92" y="1446.09">L5</tspan></text
			>
		</g>
		<g id="L4 box_2">
			<rect id="Rectangle 7_7" x="1756" y="2678" width="70" height="70" rx="20" fill="#0CA3E3" />
			<text
				id="L4_2"
				fill="white"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="36"
				letter-spacing="0em"><tspan x="1769.33" y="2726.09">L4</tspan></text
			>
		</g>
		<g id="L2a box">
			<rect id="Rectangle 7_8" x="1494" y="2287" width="70" height="70" rx="20" fill="#D81159" />
			<text
				id="L2a"
				fill="white"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="36"
				letter-spacing="0em"><tspan x="1497.83" y="2335.09">L2a</tspan></text
			>
		</g>
		<g id="L2a box_2">
			<rect id="Rectangle 7_9" x="2945" y="1202" width="70" height="70" rx="20" fill="#D81159" />
			<text
				id="L2a_2"
				fill="white"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="36"
				letter-spacing="0em"><tspan x="2948.83" y="1250.09">L2a</tspan></text
			>
		</g>
		<g id="L3 box_2">
			<rect id="Rectangle 7_10" x="1311" y="1494" width="70" height="70" rx="20" fill="#7813A8" />
			<text
				id="L3_2"
				fill="white"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="36"
				letter-spacing="0em"><tspan x="1324.41" y="1542.09">L3</tspan></text
			>
		</g>
		<g id="M2 box_2">
			<rect id="Rectangle 7_11" x="2143" y="74" width="70" height="70" rx="20" fill="#1C48E2" />
			<text
				id="M2_2"
				fill="white"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="36"
				letter-spacing="0em"><tspan x="2151.09" y="122.091">M2</tspan></text
			>
		</g>
		<g id="M1 box">
			<rect id="Rectangle 7_12" x="460" y="396" width="70" height="70" rx="20" fill="#079F4D" />
			<text
				id="M1"
				fill="white"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="36"
				letter-spacing="0em"><tspan x="470.619" y="444.091">M1</tspan></text
			>
		</g>
		<g id="M3 box">
			<rect id="Rectangle 7_13" x="550" y="396" width="70" height="70" rx="20" fill="#FF0000" />
			<text
				id="M3"
				fill="white"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="36"
				letter-spacing="0em"><tspan x="557.525" y="444.091">M3</tspan></text
			>
		</g>
		<g id="M1 box_2">
			<rect id="Rectangle 7_14" x="1720" y="2287" width="70" height="70" rx="20" fill="#079F4D" />
			<text
				id="M1_2"
				fill="white"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="36"
				letter-spacing="0em"><tspan x="1730.62" y="2335.09">M1</tspan></text
			>
		</g>
		<g id="L1 box_2">
			<rect id="Rectangle 7_15" x="1847" y="1086" width="70" height="70" rx="20" fill="#DDB011" />
			<text
				id="L1_2"
				fill="#1E1E1E"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="36"
				letter-spacing="0em"><tspan x="1864.33" y="1134.09">L1</tspan></text
			>
		</g>
		<g id="L2 box">
			<rect id="Rectangle 7_16" x="1658" y="2682" width="70" height="70" rx="20" fill="#D81159" />
			<text
				id="L2"
				fill="white"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="36"
				letter-spacing="0em"><tspan x="1671.98" y="2730.09">L2</tspan></text
			>
		</g>
		<g id="L2 box_2">
			<rect id="Rectangle 7_17" x="1945" y="1089" width="70" height="70" rx="20" fill="#D81159" />
			<text
				id="L2_2"
				fill="white"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="36"
				letter-spacing="0em"><tspan x="1958.98" y="1137.09">L2</tspan></text
			>
		</g>
		<g id="Legend">
			<path
				id="Line 52"
				d="M323 2561.2L402.087 2500"
				stroke="#D9D9D9"
				stroke-width="10"
				stroke-dasharray="10 10"
			/>
			<path
				id="Line 28"
				d="M193 1970H505"
				stroke="#079F4D"
				stroke-width="30"
				stroke-linecap="square"
			/>
			<path
				id="Line 38"
				d="M193 2220H505"
				stroke="#079F4D"
				stroke-width="30"
				stroke-linecap="square"
			/>
			<path
				id="Line 29"
				d="M193 1999H505"
				stroke="#1C48E2"
				stroke-width="30"
				stroke-linecap="square"
			/>
			<path
				id="Line 55"
				d="M193 2029H505"
				stroke="#FF0000"
				stroke-width="30"
				stroke-linecap="square"
			/>
			<path
				id="Line 39"
				d="M193 2392H505"
				stroke="#1C48E2"
				stroke-width="30"
				stroke-linecap="square"
			/>
			<g id="Group 17">
				<path
					id="Line 30"
					d="M183 2095H515"
					stroke="#DDB011"
					stroke-width="10"
					stroke-linecap="square"
				/>
				<path
					id="Line 53"
					d="M183 2075H515"
					stroke="#DDB011"
					stroke-width="10"
					stroke-linecap="square"
				/>
			</g>
			<g id="Group 18">
				<path
					id="Line 30_2"
					d="M183 2122H515"
					stroke="#D81159"
					stroke-width="10"
					stroke-linecap="square"
				/>
				<path
					id="Line 53_2"
					d="M183 2102H515"
					stroke="#D81159"
					stroke-width="10"
					stroke-linecap="square"
				/>
			</g>
			<g id="Group 20">
				<path
					id="Line 30_3"
					d="M183 2304H515"
					stroke="#D81159"
					stroke-width="10"
					stroke-linecap="square"
				/>
				<path
					id="Line 53_3"
					d="M183 2284H515"
					stroke="#D81159"
					stroke-width="10"
					stroke-linecap="square"
				/>
			</g>
			<g id="Group 19">
				<path
					id="Line 30_4"
					d="M183 2149H515"
					stroke="#7813A8"
					stroke-width="10"
					stroke-linecap="square"
				/>
				<path
					id="Line 53_4"
					d="M183 2129H515"
					stroke="#7813A8"
					stroke-width="10"
					stroke-linecap="square"
				/>
			</g>
			<g id="Group 22">
				<path
					id="Line 30_5"
					d="M183 2174H515"
					stroke="#0CA3E3"
					stroke-width="10"
					stroke-linecap="square"
				/>
				<path
					id="Line 53_5"
					d="M183 2154H515"
					stroke="#0CA3E3"
					stroke-width="10"
					stroke-linecap="square"
				/>
			</g>
			<g id="Group 21">
				<path
					id="Line 30_6"
					d="M183 2577H515"
					stroke="#7813A8"
					stroke-width="10"
					stroke-linecap="square"
				/>
				<path
					id="Line 53_6"
					d="M183 2557H515"
					stroke="#7813A8"
					stroke-width="10"
					stroke-linecap="square"
				/>
			</g>
			<path
				id="Line 40"
				d="M349 2455V2344"
				stroke="#DDB011"
				stroke-width="30"
				stroke-linecap="square"
			/>
			<rect id="Rectangle 32_2" x="393" y="2477" width="30" height="141" fill="#1E1E1E" />
			<path
				id="Line 53_7"
				d="M418 2613L418 2482"
				stroke="#0CA3E3"
				stroke-width="10"
				stroke-linecap="square"
			/>
			<path
				id="Line 54"
				d="M398 2613L398 2482"
				stroke="#0CA3E3"
				stroke-width="10"
				stroke-linecap="square"
			/>
			<text
				id="Metro Line"
				fill="#D9D9D9"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="40"
				letter-spacing="0em"><tspan x="527" y="2013.55">Metro Line</tspan></text
			>
			<text
				id="Local Trains Line"
				fill="#D9D9D9"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="40"
				letter-spacing="0em"><tspan x="527" y="2135.55">Local Trains Line</tspan></text
			>
			<text
				id="Station"
				fill="#D9D9D9"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="40"
				letter-spacing="0em"><tspan x="527" y="2233.55">Station</tspan></text
			>
			<text
				id="Interchange station"
				fill="#D9D9D9"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="40"
				letter-spacing="0em"><tspan x="527" y="2405.55">Interchange station</tspan></text
			>
			<text
				id="Out-of-station interchange"
				fill="#D9D9D9"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="40"
				letter-spacing="0em"
				><tspan x="527" y="2530.55">Out-of-station </tspan><tspan x="527" y="2578.55"
					>interchange</tspan
				></text
			>
			<text
				id="Change for ferry"
				fill="#D9D9D9"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="40"
				letter-spacing="0em"><tspan x="527" y="2682.55">Change for ferry</tspan></text
			>
			<text
				id="Change for cable car"
				fill="#D9D9D9"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="40"
				letter-spacing="0em"><tspan x="527" y="2769.55">Change for cable car</tspan></text
			>
			<text
				id="Terminal station"
				fill="#D9D9D9"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="40"
				letter-spacing="0em"><tspan x="527" y="2307.55">Terminal station</tspan></text
			>
			<g id="Station Both">
				<circle id="Ellipse 17" cx="349" cy="2392" r="13" fill="#1E1E1E" />
			</g>
			<g id="Terminal Station Horizontal">
				<rect
					id="Rectangle 23"
					x="494"
					y="2304"
					width="20"
					height="20"
					transform="rotate(-90 494 2304)"
					fill="#1E1E1E"
				/>
			</g>
			<g id="Station Horizontal">
				<circle
					id="Ellipse 17_2"
					cx="349"
					cy="2220"
					r="13"
					transform="rotate(-90 349 2220)"
					fill="#1E1E1E"
				/>
			</g>
			<g id="Station Horizontal_2">
				<circle
					id="Ellipse 17_3"
					cx="324"
					cy="2567"
					r="13"
					transform="rotate(-90 324 2567)"
					fill="#1E1E1E"
				/>
			</g>
			<g id="Station Vertical">
				<circle id="Ellipse 17_4" cx="408" cy="2502" r="13" fill="#1E1E1E" />
			</g>
		</g>
		<g id="Station Vertical_2">
			<circle id="Ellipse 17_5" cx="1626" cy="2257" r="13" fill="#3C3C3C" />
		</g>
		<g id="Station Vertical_3">
			<circle id="Ellipse 17_6" cx="1493" cy="1983" r="13" fill="#1E1E1E" />
		</g>
		<g id="Station Vertical_4">
			<circle id="Ellipse 17_7" cx="1463" cy="1531" r="13" fill="#1E1E1E" />
		</g>
		<g id="Station Vertical_5">
			<circle id="Ellipse 17_8" cx="1493" cy="1531" r="13" fill="#1E1E1E" />
		</g>
		<g id="Station Vertical_6">
			<circle id="Ellipse 17_9" cx="1596" cy="2257" r="13" fill="#3C3C3C" />
		</g>
		<g id="Station Vertical_7">
			<circle id="Ellipse 17_10" cx="1463" cy="1352" r="13" fill="#1E1E1E" />
		</g>
		<g id="Station Vertical_8">
			<circle id="Ellipse 17_11" cx="1463" cy="1184" r="13" fill="#1E1E1E" />
		</g>
		<g id="Station Vertical_9">
			<circle id="Ellipse 17_12" cx="1493" cy="1352" r="13" fill="#1E1E1E" />
		</g>
		<g id="Terminal Station Both">
			<rect id="Rectangle 22" x="1336" y="1585" width="20" height="20" fill="#1E1E1E" />
		</g>
		<g id="Terminal Station Vertical">
			<rect id="Rectangle 23_2" x="1616" y="2711" width="20" height="20" fill="#1E1E1E" />
		</g>
		<g id="Terminal Station Vertical_2">
			<rect id="Rectangle 23_3" x="1586" y="2711" width="20" height="20" fill="#1E1E1E" />
		</g>
		<g id="Terminal Station Vertical_3">
			<rect id="Rectangle 23_4" x="1745" y="2247" width="20" height="20" fill="#3C3C3C" />
		</g>
		<g id="Station Horizontal_3">
			<circle
				id="Ellipse 17_13"
				cx="1775"
				cy="1236"
				r="13"
				transform="rotate(-90 1775 1236)"
				fill="#3C3C3C"
			/>
		</g>
		<g id="Station Horizontal_4">
			<circle
				id="Ellipse 17_14"
				cx="2083"
				cy="1236"
				r="13"
				transform="rotate(-90 2083 1236)"
				fill="#3C3C3C"
			/>
		</g>
		<g id="Station Horizontal_5">
			<circle
				id="Ellipse 17_15"
				cx="1987"
				cy="944"
				r="13"
				transform="rotate(-90 1987 944)"
				fill="#3C3C3C"
			/>
		</g>
		<g id="Terminal Station Horizontal_2">
			<rect
				id="Rectangle 23_5"
				x="142"
				y="954"
				width="20"
				height="20"
				transform="rotate(-90 142 954)"
				fill="#1E1E1E"
			/>
		</g>
		<g id="Station Vertical_10">
			<circle id="Ellipse 17_16" cx="2243" cy="792" r="13" fill="#3C3C3C" />
		</g>
		<g id="Station Vertical_11">
			<circle id="Ellipse 17_17" cx="2243" cy="569" r="13" fill="#3C3C3C" />
		</g>
		<g id="Station Vertical_12">
			<circle id="Ellipse 17_18" cx="2243" cy="345" r="13" fill="#1E1E1E" />
		</g>
		<g id="Terminal Station Vertical_4">
			<rect id="Rectangle 23_6" x="2233" y="99" width="20" height="20" fill="#1E1E1E" />
		</g>
		<g id="Station Vertical_13">
			<circle id="Ellipse 17_19" cx="819" cy="1260" r="13" fill="#1E1E1E" />
		</g>
		<g id="Station Vertical_14">
			<circle id="Ellipse 17_20" cx="819" cy="1436" r="13" fill="#1E1E1E" />
		</g>
		<g id="Station Both_2">
			<circle id="Ellipse 17_21" cx="1755" cy="1847" r="13" fill="#3C3C3C" />
		</g>
		<g id="Station Both_3">
			<circle id="Ellipse 17_22" cx="1755" cy="1877" r="13" fill="#3C3C3C" />
		</g>
		<g id="Station Both_4">
			<circle id="Ellipse 17_23" cx="1755" cy="1907" r="13" fill="#3C3C3C" />
		</g>
		<g id="Terminal Station Horizontal_3">
			<rect
				id="Rectangle 23_7"
				x="1977"
				y="984"
				width="20"
				height="20"
				transform="rotate(-90 1977 984)"
				fill="#3C3C3C"
			/>
		</g>
		<g id="Terminal Station Vertical_5">
			<rect id="Rectangle 23_8" x="2029" y="1113" width="20" height="20" fill="#3C3C3C" />
		</g>
		<g id="Terminal Station Vertical_6">
			<rect id="Rectangle 23_9" x="2059" y="1113" width="20" height="20" fill="#3C3C3C" />
		</g>
		<g id="Station Vertical_15">
			<circle id="Ellipse 17_24" cx="819" cy="1084" r="13" fill="#1E1E1E" />
		</g>
		<path
			id="Metro 3"
			on:click={() => {
				if ($allActive) {
					setAll(false);
					$m3Active = true;
				} else {
					setAll(true);
				}
			}}
			class="m3 line"
			class:dim={!$m3Active}
			d="M974 526H491C435.772 526 391 570.772 391 626V784C391 839.228 435.772 884 491 884H974C1029.23 884 1074 839.228 1074 784V626C1074 570.772 1029.23 526 974 526Z"
			stroke="#FF0000"
			stroke-width="30"
		/>
		<path
			id="Metro 1_2"
			on:click={() => {
				if ($allActive) {
					setAll(false);
					$m1Active = true;
				} else {
					setAll(true);
				}
			}}
			class="m1 line"
			class:dim={!$m1Active}
			d="M974 496H491C419.203 496 361 554.203 361 626V784C361 855.797 419.203 914 491 914H974C1045.8 914 1104 855.797 1104 784V626C1104 554.203 1045.8 496 974 496Z"
			stroke="#079F4D"
			stroke-width="30"
		/>
		<g id="Direction arrow">
			<mask
				id="mask0_425_170"
				style="mask-type:alpha"
				maskUnits="userSpaceOnUse"
				x="527"
				y="511"
				width="32"
				height="30"
			>
				<rect id="Rectangle 24" x="527" y="511" width="32" height="30" fill="#D9D9D9" />
			</mask>
			<g mask="url(#mask0_425_170)">
				<path
					id="Line 54_2"
					d="M542 511L552.964 526L542 541"
					stroke="#1E1E1E"
					stroke-width="10"
					stroke-linecap="square"
				/>
			</g>
		</g>
		<g id="Direction arrow_2">
			<mask
				id="mask1_425_170"
				style="mask-type:alpha"
				maskUnits="userSpaceOnUse"
				x="871"
				y="511"
				width="32"
				height="30"
			>
				<rect id="Rectangle 24_2" x="871" y="511" width="32" height="30" fill="#D9D9D9" />
			</mask>
			<g mask="url(#mask1_425_170)">
				<path
					id="Line 54_3"
					d="M886 511L896.964 526L886 541"
					stroke="#1E1E1E"
					stroke-width="10"
					stroke-linecap="square"
				/>
			</g>
		</g>
		<g id="Direction arrow_3">
			<mask
				id="mask2_425_170"
				style="mask-type:alpha"
				maskUnits="userSpaceOnUse"
				x="929"
				y="869"
				width="32"
				height="30"
			>
				<rect
					id="Rectangle 24_3"
					x="961"
					y="899"
					width="32"
					height="30"
					transform="rotate(-180 961 899)"
					fill="#D9D9D9"
				/>
			</mask>
			<g mask="url(#mask2_425_170)">
				<path
					id="Line 54_4"
					d="M946 899L935.036 884L946 869"
					stroke="#1E1E1E"
					stroke-width="10"
					stroke-linecap="square"
				/>
			</g>
		</g>
		<g id="Direction arrow_4">
			<mask
				id="mask3_425_170"
				style="mask-type:alpha"
				maskUnits="userSpaceOnUse"
				x="376"
				y="678"
				width="30"
				height="32"
			>
				<rect
					id="Rectangle 24_4"
					x="376"
					y="710"
					width="32"
					height="30"
					transform="rotate(-90 376 710)"
					fill="#D9D9D9"
				/>
			</mask>
			<g mask="url(#mask3_425_170)">
				<path
					id="Line 54_5"
					d="M376 695L391 684.036L406 695"
					stroke="#1E1E1E"
					stroke-width="10"
					stroke-linecap="square"
				/>
			</g>
		</g>
		<g id="Direction arrow_5">
			<mask
				id="mask4_425_170"
				style="mask-type:alpha"
				maskUnits="userSpaceOnUse"
				x="346"
				y="680"
				width="30"
				height="32"
			>
				<rect
					id="Rectangle 24_5"
					x="376"
					y="680"
					width="32"
					height="30"
					transform="rotate(90 376 680)"
					fill="#D9D9D9"
				/>
			</mask>
			<g mask="url(#mask4_425_170)">
				<path
					id="Line 54_6"
					d="M376 695L361 705.964L346 695"
					stroke="#1E1E1E"
					stroke-width="10"
					stroke-linecap="square"
				/>
			</g>
		</g>
		<g id="Direction arrow_6">
			<mask
				id="mask5_425_170"
				style="mask-type:alpha"
				maskUnits="userSpaceOnUse"
				x="931"
				y="899"
				width="32"
				height="30"
			>
				<rect id="Rectangle 24_6" x="931" y="899" width="32" height="30" fill="#D9D9D9" />
			</mask>
			<g mask="url(#mask5_425_170)">
				<path
					id="Line 54_7"
					d="M946 899L956.964 914L946 929"
					stroke="#1E1E1E"
					stroke-width="10"
					stroke-linecap="square"
				/>
			</g>
		</g>
		<g id="Direction arrow_7">
			<mask
				id="mask6_425_170"
				style="mask-type:alpha"
				maskUnits="userSpaceOnUse"
				x="525"
				y="481"
				width="32"
				height="30"
			>
				<rect
					id="Rectangle 24_7"
					x="557"
					y="511"
					width="32"
					height="30"
					transform="rotate(-180 557 511)"
					fill="#D9D9D9"
				/>
			</mask>
			<g mask="url(#mask6_425_170)">
				<path
					id="Line 54_8"
					d="M542 511L531.036 496L542 481"
					stroke="#1E1E1E"
					stroke-width="10"
					stroke-linecap="square"
				/>
			</g>
		</g>
		<g id="Direction arrow_8">
			<mask
				id="mask7_425_170"
				style="mask-type:alpha"
				maskUnits="userSpaceOnUse"
				x="869"
				y="481"
				width="32"
				height="30"
			>
				<rect
					id="Rectangle 24_8"
					x="901"
					y="511"
					width="32"
					height="30"
					transform="rotate(-180 901 511)"
					fill="#D9D9D9"
				/>
			</mask>
			<g mask="url(#mask7_425_170)">
				<path
					id="Line 54_9"
					d="M886 511L875.036 496L886 481"
					stroke="#1E1E1E"
					stroke-width="10"
					stroke-linecap="square"
				/>
			</g>
		</g>
		<g id="Station Horizontal_6">
			<circle
				id="Ellipse 17_25"
				cx="737"
				cy="914"
				r="13"
				transform="rotate(-90 737 914)"
				fill="#1E1E1E"
			/>
		</g>
		<g id="Station Horizontal_7">
			<circle
				id="Ellipse 17_26"
				cx="737"
				cy="884"
				r="13"
				transform="rotate(-90 737 884)"
				fill="#1E1E1E"
			/>
		</g>
		<g id="Station Horizontal_8">
			<circle
				id="Ellipse 17_27"
				cx="733"
				cy="496"
				r="13"
				transform="rotate(-90 733 496)"
				fill="#1E1E1E"
			/>
		</g>
		<g id="Station Horizontal_9">
			<circle
				id="Ellipse 17_28"
				cx="733"
				cy="526"
				r="13"
				transform="rotate(-90 733 526)"
				fill="#1E1E1E"
			/>
		</g>
		<g id="Station Vertical_16">
			<circle id="Ellipse 17_29" cx="1074" cy="705" r="13" fill="#1E1E1E" />
		</g>
		<g id="Station Vertical_17">
			<circle id="Ellipse 17_30" cx="1104" cy="705" r="13" fill="#1E1E1E" />
		</g>
		<g id="Station Horizontal_10">
			<circle
				id="Ellipse 17_31"
				cx="516"
				cy="884"
				r="13"
				transform="rotate(-90 516 884)"
				fill="#1E1E1E"
			/>
		</g>
		<g id="Station Horizontal_11">
			<circle
				id="Ellipse 17_32"
				cx="516"
				cy="914"
				r="13"
				transform="rotate(-90 516 914)"
				fill="#1E1E1E"
			/>
		</g>
		<g id="Station Horizontal_12">
			<circle
				id="Ellipse 17_33"
				cx="516"
				cy="944"
				r="13"
				transform="rotate(-90 516 944)"
				fill="#1E1E1E"
			/>
		</g>
		<g id="Station Horizontal_13">
			<circle
				id="Ellipse 17_34"
				cx="737"
				cy="944"
				r="13"
				transform="rotate(-90 737 944)"
				fill="#1E1E1E"
			/>
		</g>
		<g id="Station Horizontal_14">
			<circle
				id="Ellipse 17_35"
				cx="2286"
				cy="1847"
				r="13"
				transform="rotate(-90 2286 1847)"
				fill="#3C3C3C"
			/>
		</g>
		<g id="Station Horizontal_15">
			<circle
				id="Ellipse 17_36"
				cx="2537"
				cy="1847"
				r="13"
				transform="rotate(-90 2537 1847)"
				fill="#1E1E1E"
			/>
		</g>
		<g id="Station Horizontal_16">
			<circle
				id="Ellipse 17_37"
				cx="2537"
				cy="1206"
				r="13"
				transform="rotate(-90 2537 1206)"
				fill="#3C3C3C"
			/>
		</g>
		<g id="Station Horizontal_17">
			<circle
				id="Ellipse 17_38"
				cx="2788"
				cy="1847"
				r="13"
				transform="rotate(-90 2788 1847)"
				fill="#1E1E1E"
			/>
		</g>
		<g id="Station Horizontal_18">
			<circle
				id="Ellipse 17_39"
				cx="2286"
				cy="1877"
				r="13"
				transform="rotate(-90 2286 1877)"
				fill="#3C3C3C"
			/>
		</g>
		<g id="Station Horizontal_19">
			<circle
				id="Ellipse 17_40"
				cx="2537"
				cy="1877"
				r="13"
				transform="rotate(-90 2537 1877)"
				fill="#1E1E1E"
			/>
		</g>
		<g id="Station Horizontal_20">
			<circle
				id="Ellipse 17_41"
				cx="2537"
				cy="1236"
				r="13"
				transform="rotate(-90 2537 1236)"
				fill="#3C3C3C"
			/>
		</g>
		<g id="Station Horizontal_21">
			<circle
				id="Ellipse 17_42"
				cx="2788"
				cy="1877"
				r="13"
				transform="rotate(-90 2788 1877)"
				fill="#1E1E1E"
			/>
		</g>
		<g id="Station Horizontal_22">
			<circle
				id="Ellipse 17_43"
				cx="2286"
				cy="1907"
				r="13"
				transform="rotate(-90 2286 1907)"
				fill="#3C3C3C"
			/>
		</g>
		<g id="Station Horizontal_23">
			<circle
				id="Ellipse 17_44"
				cx="2537"
				cy="1907"
				r="13"
				transform="rotate(-90 2537 1907)"
				fill="#1E1E1E"
			/>
		</g>
		<g id="Station Horizontal_24">
			<circle
				id="Ellipse 17_45"
				cx="2788"
				cy="1907"
				r="13"
				transform="rotate(-90 2788 1907)"
				fill="#1E1E1E"
			/>
		</g>
		<g id="Station Vertical_18">
			<circle id="Ellipse 17_46" cx="2885" cy="1503" r="13" fill="#1E1E1E" />
		</g>
		<g id="Station Vertical_19">
			<circle id="Ellipse 17_47" cx="2915" cy="1503" r="13" fill="#1E1E1E" />
		</g>
		<g id="Terminal Station Vertical_7">
			<rect id="Rectangle 23_10" x="2845" y="1493" width="20" height="20" fill="#1E1E1E" />
		</g>
		<g id="Terminal Station Vertical_8">
			<rect id="Rectangle 23_11" x="2935" y="1493" width="20" height="20" fill="#1E1E1E" />
		</g>
		<rect id="Rectangle 38" x="1946" y="1231" width="65" height="10" fill="#3C3C3C" />
		<g id="Station Both_5">
			<circle id="Ellipse 17_48" cx="1463" cy="944" r="13" fill="#1E1E1E" />
		</g>
		<g id="Terminal Station Both_2">
			<rect id="Rectangle 22_2" x="1124" y="695" width="20" height="20" fill="#1E1E1E" />
		</g>
		<line
			id="Text cross"
			x1="2413.5"
			y1="1758.5"
			x2="2660.5"
			y2="1758.5"
			stroke="#9C1010"
			stroke-width="5"
			stroke-linecap="round"
		/>
		<line
			id="Text cross_2"
			x1="2476.5"
			y1="1805.5"
			x2="2601.5"
			y2="1805.5"
			stroke="#9C1010"
			stroke-width="5"
			stroke-linecap="round"
		/>
		<g id="Closed station / cross">
			<mask
				id="mask9_425_170"
				style="mask-type:alpha"
				maskUnits="userSpaceOnUse"
				x="2522"
				y="1832"
				width="30"
				height="30"
			>
				<rect id="Rectangle 57" x="2522" y="1832" width="30" height="30" fill="#D9D9D9" />
			</mask>
			<g mask="url(#mask9_425_170)">
				<path
					id="Line 67"
					d="M2526 1858L2537 1847M2548 1836L2537 1847M2537 1847L2548 1858M2537 1847L2526 1836"
					stroke="#9C1010"
					stroke-width="5"
					stroke-linecap="round"
				/>
			</g>
		</g>
		<g id="Closed station / cross_2">
			<mask
				id="mask10_425_170"
				style="mask-type:alpha"
				maskUnits="userSpaceOnUse"
				x="2522"
				y="1862"
				width="30"
				height="30"
			>
				<rect id="Rectangle 57_2" x="2522" y="1862" width="30" height="30" fill="#D9D9D9" />
			</mask>
			<g mask="url(#mask10_425_170)">
				<path
					id="Line 67_2"
					d="M2526 1888L2537 1877M2548 1866L2537 1877M2537 1877L2548 1888M2537 1877L2526 1866"
					stroke="#9C1010"
					stroke-width="5"
					stroke-linecap="round"
				/>
			</g>
		</g>
		<g id="Closed station / cross_3">
			<mask
				id="mask11_425_170"
				style="mask-type:alpha"
				maskUnits="userSpaceOnUse"
				x="2522"
				y="1892"
				width="30"
				height="30"
			>
				<rect id="Rectangle 57_3" x="2522" y="1892" width="30" height="30" fill="#D9D9D9" />
			</mask>
			<g mask="url(#mask11_425_170)">
				<path
					id="Line 67_3"
					d="M2526 1918L2537 1907M2548 1896L2537 1907M2537 1907L2548 1918M2537 1907L2526 1896"
					stroke="#9C1010"
					stroke-width="5"
					stroke-linecap="round"
				/>
			</g>
		</g>
		<g id="Closure warning">
			<g
				id="The Spruce Basin Village is closed due to the ongoing construction of the eastern vestibule. Trains pass through the station. We apologize for the inconvenience"
			>
				<text
					fill="white"
					xml:space="preserve"
					style="white-space: pre"
					font-family="Inter"
					font-size="40"
					letter-spacing="0em"
					><tspan x="2355" y="2585.55">The </tspan><tspan x="2840.43" y="2585.55">
						is closed
					</tspan><tspan x="2355" y="2633.55">due to the ongoing construction of </tspan><tspan
						x="2355"
						y="2681.55"
						>the eastern vestibule. Trains pass
					</tspan><tspan x="2355" y="2729.55">through the station. We apologize </tspan><tspan
						x="2355"
						y="2777.55">for the inconvenience</tspan
					></text
				>
				<text
					fill="white"
					xml:space="preserve"
					style="white-space: pre"
					font-family="Inter"
					font-size="40"
					font-weight="bold"
					letter-spacing="0em"><tspan x="2438.83" y="2585.55">Spruce Basin Village</tspan></text
				>
			</g>
			<text
				id="Local Trains station closure"
				fill="white"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="48"
				font-weight="bold"
				letter-spacing="0em"><tspan x="2355" y="2491.45">Local Trains station closure</tspan></text
			>
			<text
				id="!"
				fill="white"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="256"
				letter-spacing="0em"><tspan x="2263.88" y="2708.09">!</tspan></text
			>
		</g>
		{#if !$hideFareZones}
			<text
				id="Zone 0"
				fill="#3C3C3C"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="64"
				letter-spacing="0em"><tspan x="665" y="1884.77">ZONE 0</tspan></text
			>
			<text
				id="Zone 0_2"
				fill="#3C3C3C"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="64"
				letter-spacing="0em"><tspan x="1349" y="457.773">ZONE 0</tspan></text
			>
			<text
				id="Zone 2"
				fill="#3C3C3C"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="64"
				letter-spacing="0em"><tspan x="2581" y="2271.77">ZONE 2</tspan></text
			>
			<text
				id="Zone 2_2"
				fill="#3C3C3C"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="64"
				letter-spacing="0em"><tspan x="2431" y="251.773">ZONE 2</tspan></text
			>
			<text
				id="Zone 1"
				fill="#1E1E1E"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="64"
				letter-spacing="0em"><tspan x="2011" y="1514.77">ZONE 1</tspan></text
			>
			<text
				id="Zone 3"
				fill="#1E1E1E"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="64"
				letter-spacing="0em"><tspan x="3484" y="600.773">ZONE 3</tspan></text
			>
			<text
				id="Zone 3_2"
				fill="#1E1E1E"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="64"
				letter-spacing="0em"><tspan x="3484" y="2442.77">ZONE 3</tspan></text
			>
			<text
				id="Zone 1_2"
				fill="#1E1E1E"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="64"
				letter-spacing="0em"><tspan x="1163" y="2468.77">ZONE 1</tspan></text
			>
			<text
				id="Zone 1_3"
				fill="#1E1E1E"
				xml:space="preserve"
				style="white-space: pre"
				font-family="Inter"
				font-size="64"
				letter-spacing="0em"><tspan x="1965" y="600.773">ZONE 1</tspan></text
			>
		{/if}
		<path
			id="Local Trains 5"
			on:click={() => {
				if ($allActive) {
					setAll(false);
					$l5Active = true;
				} else {
					setAll(true);
				}
			}}
			class="l5 line"
			class:dim={!$l5Active}
			d="M2965 1493H3372.43L3806 1493"
			stroke="#FF8200"
			stroke-width="10"
			stroke-linecap="square"
		/>
		<path
			id="Local Trains 5_2"
			on:click={() => {
				if ($allActive) {
					setAll(false);
					$l5Active = true;
				} else {
					setAll(true);
				}
			}}
			class="l5 line"
			class:dim={!$l5Active}
			d="M2966 1513H3373.43L3807 1513"
			stroke="#FF8200"
			stroke-width="10"
			stroke-linecap="square"
		/>
		<g id="Terminal Station Horizontal_4">
			<rect
				id="Rectangle 23_12"
				x="2965"
				y="1513"
				width="20"
				height="20"
				transform="rotate(-90 2965 1513)"
				fill="#1E1E1E"
			/>
		</g>
		<g id="Terminal Station Horizontal_5">
			<rect
				id="Rectangle 23_13"
				x="3786"
				y="1513"
				width="20"
				height="20"
				transform="rotate(-90 3786 1513)"
				fill="#3C3C3C"
			/>
		</g>
		<g id="Station Horizontal_25">
			<circle
				id="Ellipse 17_49"
				cx="3497"
				cy="1503"
				r="13"
				transform="rotate(-90 3497 1503)"
				fill="#3C3C3C"
			/>
		</g>
		<g id="Station Horizontal_26">
			<circle
				id="Ellipse 17_50"
				cx="3211"
				cy="1503"
				r="13"
				transform="rotate(-90 3211 1503)"
				fill="#1E1E1E"
			/>
		</g>
		<g id="Cable Car Sign">
			<g id="Polygon 7">
				<path
					fill-rule="evenodd"
					clip-rule="evenodd"
					d="M3675.06 1416.59C3674.43 1414.46 3672.48 1413 3670.26 1413L3667 1413L3664 1413L3660.74 1413C3658.52 1413 3656.57 1414.46 3655.94 1416.59L3652.83 1427.18C3652.29 1429.02 3652.29 1430.98 3652.83 1432.82L3655.94 1443.41C3656.57 1445.54 3658.52 1447 3660.74 1447H3670.26C3672.48 1447 3674.43 1445.54 3675.06 1443.41L3678.17 1432.82C3678.71 1430.98 3678.71 1429.02 3678.17 1427.18L3675.06 1416.59ZM3661.96 1416C3661.09 1416 3660.32 1416.56 3660.05 1417.39L3656.98 1426.94C3656.34 1428.93 3656.34 1431.07 3656.98 1433.06L3660.05 1442.61C3660.32 1443.44 3661.09 1444 3661.96 1444H3669.49C3670.38 1444 3671.17 1443.41 3671.41 1442.55L3674.22 1432.75C3674.73 1430.95 3674.73 1429.05 3674.22 1427.25L3671.41 1417.45C3671.17 1416.59 3670.38 1416 3669.49 1416H3661.96Z"
					fill="#D9D9D9"
				/>
				<path d="M3664 1405V1413L3667 1413V1403.5L3664 1405Z" fill="#D9D9D9" />
				<path
					d="M3664 1405L3667 1403.5L3674 1400V1400C3674 1399.08 3673.03 1398.48 3672.21 1398.89L3664 1403L3657.49 1406.25C3657.19 1406.4 3657 1406.71 3657 1407.05V1407.05C3657 1407.72 3657.7 1408.15 3658.29 1407.85L3664 1405Z"
					fill="#D9D9D9"
				/>
			</g>
		</g>
		<g id="Cable Car Sign_2">
			<g id="Polygon 7_2">
				<path
					fill-rule="evenodd"
					clip-rule="evenodd"
					d="M2481.06 1949.59C2480.43 1947.46 2478.48 1946 2476.26 1946L2473 1946L2470 1946L2466.74 1946C2464.52 1946 2462.57 1947.46 2461.94 1949.59L2458.83 1960.18C2458.29 1962.02 2458.29 1963.98 2458.83 1965.82L2461.94 1976.41C2462.57 1978.54 2464.52 1980 2466.74 1980H2476.26C2478.48 1980 2480.43 1978.54 2481.06 1976.41L2484.17 1965.82C2484.71 1963.98 2484.71 1962.02 2484.17 1960.18L2481.06 1949.59ZM2467.96 1949C2467.09 1949 2466.32 1949.56 2466.05 1950.39L2462.98 1959.94C2462.34 1961.93 2462.34 1964.07 2462.98 1966.06L2466.05 1975.61C2466.32 1976.44 2467.09 1977 2467.96 1977H2475.49C2476.38 1977 2477.17 1976.41 2477.41 1975.55L2480.22 1965.75C2480.73 1963.95 2480.73 1962.05 2480.22 1960.25L2477.41 1950.45C2477.17 1949.59 2476.38 1949 2475.49 1949H2467.96Z"
					fill="#D9D9D9"
				/>
				<path d="M2470 1938V1946L2473 1946V1936.5L2470 1938Z" fill="#D9D9D9" />
				<path
					d="M2470 1938L2473 1936.5L2480 1933V1933C2480 1932.08 2479.03 1931.48 2478.21 1931.89L2470 1936L2463.49 1939.25C2463.19 1939.4 2463 1939.71 2463 1940.05V1940.05C2463 1940.72 2463.7 1941.15 2464.29 1940.85L2470 1938Z"
					fill="#D9D9D9"
				/>
			</g>
		</g>
		<g id="Boat symbol">
			<path
				id="Polygon 8"
				fill-rule="evenodd"
				clip-rule="evenodd"
				d="M1127.8 1086.18C1127.8 1083.17 1130.25 1080.72 1133.26 1080.72H1137.36C1140.47 1080.72 1143 1078.19 1143 1075.08V1072.88C1143 1071.84 1143.84 1071 1144.88 1071H1171.6C1176.79 1071 1181 1075.21 1181 1080.4V1080.72H1194.74C1197.65 1080.72 1200 1083.07 1200 1085.98V1085.98C1200 1088.04 1198.8 1089.91 1196.92 1090.76L1182.85 1097.16C1181.63 1097.71 1180.31 1098 1178.96 1098H1145.48C1143.86 1098 1142.26 1097.58 1140.84 1096.77L1130.56 1090.93C1128.85 1089.96 1127.8 1088.15 1127.8 1086.18V1086.18ZM1146.8 1074.24V1078.56H1150.6V1074.24H1146.8ZM1154.4 1078.56V1074.24H1158.2V1078.56H1154.4ZM1162 1074.24V1078.56H1165.8V1074.24H1162ZM1169.6 1078.56V1074.24H1173.4V1078.56H1169.6Z"
				fill="#D9D9D9"
			/>
			<path
				id="Line 78"
				d="M1124 1091.52C1124 1091.52 1129.5 1095.84 1133.5 1095.84C1137.5 1095.84 1139 1091.52 1143 1091.52C1147 1091.52 1148.5 1095.84 1152.5 1095.84C1156.5 1095.84 1158 1091.52 1162 1091.52C1166 1091.52 1167.5 1095.84 1171.5 1095.84C1175.5 1095.84 1177 1091.52 1181 1091.52C1185 1091.52 1186.5 1095.84 1190.5 1095.84C1194.5 1095.84 1200 1091.52 1200 1091.52"
				stroke="#BFBFBF"
				stroke-width="1.88"
				stroke-linecap="round"
			/>
		</g>
		<g id="Boat symbol_2">
			<path
				id="Polygon 8_2"
				fill-rule="evenodd"
				clip-rule="evenodd"
				d="M724.8 1262.18C724.8 1259.17 727.245 1256.72 730.262 1256.72H734.36C737.475 1256.72 740 1254.19 740 1251.08V1248.88C740 1247.84 740.841 1247 741.88 1247H768.6C773.791 1247 778 1251.21 778 1256.4V1256.72H791.744C794.646 1256.72 797 1259.07 797 1261.98V1261.98C797 1264.04 795.795 1265.91 793.919 1266.76L779.854 1273.16C778.632 1273.71 777.305 1274 775.963 1274H742.485C740.856 1274 739.255 1273.58 737.839 1272.77L727.563 1266.93C725.855 1265.96 724.8 1264.15 724.8 1262.18V1262.18ZM743.8 1250.24V1254.56H747.6V1250.24H743.8ZM751.4 1254.56V1250.24H755.2V1254.56H751.4ZM759 1250.24V1254.56H762.8V1250.24H759ZM766.6 1254.56V1250.24H770.4V1254.56H766.6Z"
				fill="#D9D9D9"
			/>
			<path
				id="Line 78_2"
				d="M721 1267.52C721 1267.52 726.504 1271.84 730.5 1271.84C734.496 1271.84 736.004 1267.52 740 1267.52C743.996 1267.52 745.504 1271.84 749.5 1271.84C753.496 1271.84 755.004 1267.52 759 1267.52C762.996 1267.52 764.504 1271.84 768.5 1271.84C772.496 1271.84 774.004 1267.52 778 1267.52C781.996 1267.52 783.504 1271.84 787.5 1271.84C791.496 1271.84 797 1267.52 797 1267.52"
				stroke="#BFBFBF"
				stroke-width="1.88"
				stroke-linecap="round"
			/>
		</g>
		<g id="Boat symbol_3">
			<path
				id="Polygon 8_3"
				fill-rule="evenodd"
				clip-rule="evenodd"
				d="M724.8 1438.18C724.8 1435.17 727.245 1432.72 730.262 1432.72H734.36C737.475 1432.72 740 1430.19 740 1427.08V1424.88C740 1423.84 740.841 1423 741.88 1423H768.6C773.791 1423 778 1427.21 778 1432.4V1432.72H791.744C794.646 1432.72 797 1435.07 797 1437.98V1437.98C797 1440.04 795.795 1441.91 793.919 1442.76L779.854 1449.16C778.632 1449.71 777.305 1450 775.963 1450H742.485C740.856 1450 739.255 1449.58 737.839 1448.77L727.563 1442.93C725.855 1441.96 724.8 1440.15 724.8 1438.18V1438.18ZM743.8 1426.24V1430.56H747.6V1426.24H743.8ZM751.4 1430.56V1426.24H755.2V1430.56H751.4ZM759 1426.24V1430.56H762.8V1426.24H759ZM766.6 1430.56V1426.24H770.4V1430.56H766.6Z"
				fill="#D9D9D9"
			/>
			<path
				id="Line 78_3"
				d="M721 1443.52C721 1443.52 726.504 1447.84 730.5 1447.84C734.496 1447.84 736.004 1443.52 740 1443.52C743.996 1443.52 745.504 1447.84 749.5 1447.84C753.496 1447.84 755.004 1443.52 759 1443.52C762.996 1443.52 764.504 1447.84 768.5 1447.84C772.496 1447.84 774.004 1443.52 778 1443.52C781.996 1443.52 783.504 1447.84 787.5 1447.84C791.496 1447.84 797 1443.52 797 1443.52"
				stroke="#BFBFBF"
				stroke-width="1.88"
				stroke-linecap="round"
			/>
		</g>
		<g id="Boat symbol_4">
			<path
				id="Polygon 8_4"
				fill-rule="evenodd"
				clip-rule="evenodd"
				d="M442.8 2670.18C442.8 2667.17 445.245 2664.72 448.262 2664.72H452.36C455.475 2664.72 458 2662.19 458 2659.08V2656.88C458 2655.84 458.841 2655 459.88 2655H486.6C491.791 2655 496 2659.21 496 2664.4V2664.72H509.744C512.646 2664.72 515 2667.07 515 2669.98V2669.98C515 2672.04 513.795 2673.91 511.919 2674.76L497.854 2681.16C496.632 2681.71 495.305 2682 493.963 2682H460.485C458.856 2682 457.255 2681.58 455.839 2680.77L445.563 2674.93C443.855 2673.96 442.8 2672.15 442.8 2670.18V2670.18ZM461.8 2658.24V2662.56H465.6V2658.24H461.8ZM469.4 2662.56V2658.24H473.2V2662.56H469.4ZM477 2658.24V2662.56H480.8V2658.24H477ZM484.6 2662.56V2658.24H488.4V2662.56H484.6Z"
				fill="#D9D9D9"
			/>
			<path
				id="Line 78_4"
				d="M439 2675.52C439 2675.52 444.504 2679.84 448.5 2679.84C452.496 2679.84 454.004 2675.52 458 2675.52C461.996 2675.52 463.504 2679.84 467.5 2679.84C471.496 2679.84 473.004 2675.52 477 2675.52C480.996 2675.52 482.504 2679.84 486.5 2679.84C490.496 2679.84 492.004 2675.52 496 2675.52C499.996 2675.52 501.504 2679.84 505.5 2679.84C509.496 2679.84 515 2675.52 515 2675.52"
				stroke="#BFBFBF"
				stroke-width="1.88"
				stroke-linecap="round"
			/>
		</g>
		<g id="Cable Car Sign_3">
			<g id="Polygon 7_3">
				<path
					fill-rule="evenodd"
					clip-rule="evenodd"
					d="M510.056 2739.59C509.43 2737.46 507.477 2736 505.259 2736L502 2736L499 2736L495.741 2736C493.523 2736 491.57 2737.46 490.944 2739.59L487.83 2750.18C487.288 2752.02 487.288 2753.98 487.83 2755.82L490.944 2766.41C491.57 2768.54 493.523 2770 495.741 2770H505.259C507.477 2770 509.43 2768.54 510.056 2766.41L513.17 2755.82C513.712 2753.98 513.712 2752.02 513.17 2750.18L510.056 2739.59ZM496.958 2739C496.089 2739 495.32 2739.56 495.054 2740.39L491.984 2749.94C491.344 2751.93 491.344 2754.07 491.984 2756.06L495.054 2765.61C495.32 2766.44 496.089 2767 496.958 2767H504.491C505.384 2767 506.169 2766.41 506.414 2765.55L509.215 2755.75C509.728 2753.95 509.728 2752.05 509.215 2750.25L506.414 2740.45C506.169 2739.59 505.384 2739 504.491 2739H496.958Z"
					fill="#D9D9D9"
				/>
				<path d="M499 2728V2736L502 2736V2726.5L499 2728Z" fill="#D9D9D9" />
				<path
					d="M499 2728L502 2726.5L509 2723V2723C509 2722.08 508.033 2721.48 507.211 2721.89L499 2726L492.494 2729.25C492.191 2729.4 492 2729.71 492 2730.05V2730.05C492 2730.72 492.7 2731.15 493.294 2730.85L499 2728Z"
					fill="#D9D9D9"
				/>
			</g>
		</g>
	</g>
	<defs>
		<clipPath id="clip0_425_170">
			<rect width="3907" height="2828" fill="white" />
		</clipPath>
	</defs>
</svg>

<style>
	.line {
		cursor: pointer;
		transition: all 400ms;
	}

	.dim {
		opacity: 0.4;
	}
</style>
