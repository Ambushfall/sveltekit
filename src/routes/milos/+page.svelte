<script>
	import { confetti } from '@neoconfetti/svelte';
	import { reduced_motion } from '../sverdle/reduced-motion';
</script>

<svelte:head>
	<title>Milos</title>
	<meta name="description" content="Webpage made for the one and only" />
</svelte:head>
<h1>Welcome to Milos's webpage</h1>
<div
	use:confetti={{
		particleCount: $reduced_motion ? 0 : undefined,
		force: 0.7,
		stageWidth: window.innerWidth,
		stageHeight: window.innerHeight,
		colors: ['#ff3e00', '#40b3ff', '#676778']
	}}
/>
