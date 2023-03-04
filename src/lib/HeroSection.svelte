<script lang="ts">
	import { onMount } from 'svelte';
	import Container from './Container.svelte';
	import HeroImage from '$lib/assets/HeroImage.png';

	const GateText = ['NFTs', 'Tokens', 'POAPs', 'Snapshot', 'Otterspace Badges'];

	const ToolText = ['Notion', 'Google Drive', 'CharmVerse', 'Discord'];
	let gateCounter: number = 0;
	let toolCounter: number = 0;

	let currentGate: string = GateText[0];
	let currentTool: string = ToolText[0];

	function changeGateText() {
		gateCounter++;
		if (gateCounter >= GateText.length) {
			gateCounter = 0;
		}
		currentGate = GateText[gateCounter];
	}

	function changeToolText() {
		toolCounter++;
		if (toolCounter >= ToolText.length) {
			toolCounter = 0;
		}
		currentTool = ToolText[toolCounter];
	}

	onMount(() => {
		setInterval(changeGateText, 2000);
		setInterval(changeToolText, 2000);
	});
</script>

<div class="relative overflow-hidden dark:bg-darker lg:overflow-auto" id="home">
	<div class="absolute inset-x-0 top-32 lg:hidden">
		<div
			aria-hidden="true"
			class="grid grid-cols-2 -space-x-52 opacity-50 dark:opacity-60 2xl:mx-auto 2xl:max-w-6xl"
		>
			<div class="h-60 bg-gradient-to-br from-primary to-purple-400 blur-3xl dark:from-blue-700" />
			<div
				class="h-72 rounded-full bg-gradient-to-r from-cyan-400 to-sky-300 blur-3xl dark:from-transparent dark:to-indigo-600"
			/>
		</div>
	</div>
	<Container>
		<div class="relative ml-auto pt-40 xl:pt-36">
			<div class="gap-12 md:flex md:items-center">
				<div class="text-center sm:px-12 md:w-2/3 md:px-0 md:text-left lg:w-1/2">
					<h1 class="text-3xl font-black dark:text-white md:text-6xl xl:text-7xl">
						Gate access to <span class="text-secondary">{currentTool}</span> using
						<span class="text-secondary">{currentGate}</span>
					</h1>
					<div class="">
						<p class="mt-8 text-lg text-gray-700 dark:text-gray-100">
							Easily share your documents with the right people using any web3 primitive.
						</p>
						<a
							href="https://form.waitlistpanda.com/go/L0zfvXH00hvIG9DSTLUw"
							target="_blank"
							rel="noreferrer"
							class="relative mt-4 flex h-12 w-full items-center justify-center px-14 before:absolute before:inset-0 before:rounded-full before:bg-primary before:transition before:duration-300 hover:before:scale-105 active:duration-75 active:before:scale-95 sm:w-max"
						>
							<span class="relative font-semibold text-white">Sign up</span>
						</a>
					</div>
				</div>
				<div class="relative mt-20 md:mt-0 md:w-2/5 lg:w-3/5">
					<div class="-ml-6 md:-mr-72 lg:mr-0">
						<img
							class="h-full object-cover object-left dark:hidden"
							src={HeroImage}
							alt="app screenshot"
							width="1628"
							height="1233"
						/>
						<img
							class="hidden h-full object-cover object-left dark:block"
							src={HeroImage}
							alt="app screenshot"
							width="1628"
							height="1233"
						/>
					</div>
				</div>
			</div>
		</div>
	</Container>
</div>
