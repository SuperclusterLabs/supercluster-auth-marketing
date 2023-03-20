<script lang="ts">
	import { onMount } from 'svelte';
	import Container from './Container.svelte';
	import HeroImage from '$lib/assets/Hero-Image.png';

	const GateText = ['NFTs', 'Tokens', 'POAPs', 'Snapshot', 'Otterspace'];

	const ToolText = ['Notion', 'Drive', 'Asana', 'Discord', 'Trello'];
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

<div class="relative dark:bg-darker" id="home">
	<Container>
		<div class="relative ml-auto pt-40 xl:pt-36">
			<div class="gap-12 md:flex md:items-center">
				<div
					class="text-center sm:px-12 md:w-2/3 px-8 py-8 md:text-left lg:w-1/2 drop-shadow-xl bg-white rounded-3xl"
				>
					<h1 class="font-black text-4xl md:text-6xl">
						Gate access to <br />
						<h1 class="text-secondary text-5xl md:text-7xl my-4 underline underline-offset-4">
							{currentTool}
						</h1>
						using<br />
						<h1 class="text-secondary text-5xl md:text-7xl my-4 underline underline-offset-4">
							{currentGate}
						</h1>
					</h1>
					<div class="">
						<p class="mt-8 text-lg text-gray-700 dark:text-gray-100">
							Easily manage access to all your collaboration tools for your community. Your
							community deserves the tools that actually work.
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
				<div class="relative mt-20 md:mt-0 md:w-2/5">
					<div class="-ml-6 md:-mr-72 lg:mr-0">
						<img
							class="h-full object-cover object-left dark:hidden"
							src={HeroImage}
							alt="app screenshot"
						/>
					</div>
				</div>
			</div>
		</div>
	</Container>
</div>
