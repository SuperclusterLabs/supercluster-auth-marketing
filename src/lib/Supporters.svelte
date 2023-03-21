<script lang="ts">
	import Container from './Container.svelte';
	import outlierVenturesLogo from '$lib/assets/outlier-logo.png';
	import protocolLabsLogo from '$lib/assets/protocol-labs-logo.png';
</script>

<Container>
	<h2 class="text-2xl uppercase text-center font-bold mt-24">Supporters</h2>
	<div class="flex flex-row gap-8 items-center justify-center mt-8">
		<img class="w-[200px]" src={outlierVenturesLogo} alt="Outlier Ventures logo" />
		<img class="w-[200px]" src={protocolLabsLogo} alt="Protocol Labs logo" />
	</div>
</Container>
