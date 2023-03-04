<script lang="ts">
	import Container from './Container.svelte';
	import Feature from './Feature.svelte';

	// Images
	import HeaderImage from '$lib/assets/header.jpg';
	import BadgeSVG from '$lib/assets/Badge.svg';
	import NFTSVG from '$lib/assets/NFT.svg';
	import TokenSVG from '$lib/assets/Token.svg';
</script>

<div class="relative pt-32 md:pt-44" id="features">
	<Container>
		<div class="mx-auto md:w-3/5">
			<h2
				class="text-center text-3xl font-bold text-gray-900 dark:text-white md:text-4xl lg:text-5xl"
			>
				Designed for your decentralized community
			</h2>
		</div>

		<div class="mt-16 md:mt-20">
			<div
				class="relative grid rounded-3xl border border-gray-200 p-1 dark:border-gray-800 lg:grid-cols-2"
			>
				<div class="absolute inset-0 hidden h-max dark:block lg:my-auto">
					<div
						aria-hidden="true"
						class="grid grid-cols-2 -space-x-52 opacity-50 dark:opacity-70 2xl:mx-auto 2xl:max-w-6xl"
					>
						<div
							class="h-60 bg-gradient-to-br from-primary to-purple-400 blur-3xl dark:from-blue-700"
						/>
						<div
							class="h-72 rounded-full bg-gradient-to-r from-cyan-400 to-sky-300 blur-3xl dark:from-transparent dark:to-indigo-600"
						/>
					</div>
				</div>
				<div>
					<div
						class="relative flex h-full flex-col items-center justify-center gap-6 p-8 py-16 lg:py-8"
					>
						<img
							src={HeaderImage}
							alt="xp icon illustration"
							width="512"
							height="512"
							loading="lazy"
						/>
						<div class="mx-auto text-center sm:w-2/5">
							<h2 class="text-xl font-semibold text-gray-900 dark:text-white">
								Gate any of your community's content using your web3 primitives
							</h2>
						</div>
					</div>
				</div>
				<div
					class="relative grid overflow-hidden rounded-[1.25rem] bg-gray-100 p-1 dark:bg-gray-800/50 sm:grid-cols-2"
				>
					<Feature
						title="NFTs"
						description="Gate access to your content or tools using any ERC-721 or ERC-1155"
					>
						<img class="m-auto h-6 w-6 text-gray-700 dark:text-white" src={NFTSVG} alt="NFT" />
					</Feature>

					<Feature title="Tokens" description="Use your community token to gate your content">
						<img class="m-auto h-6 w-6 text-gray-700 dark:text-white" src={TokenSVG} alt="Token" />
					</Feature>

					<Feature
						title="POAPs"
						description="Ensure that only people that attended your events have access"
					>
						<img
							class="m-auto h-6 w-6 text-gray-700 dark:text-white"
							src={BadgeSVG}
							alt="POAP Badge"
						/>
					</Feature>

					<Feature
						title="Snapshot"
						description="Allow access to engaged members who vote on your Snapshot proposals"
					>
						<svg
							xmlns="http://www.w3.org/2000/svg"
							fill="none"
							viewBox="0 0 24 24"
							stroke-width="1.5"
							stroke="currentColor"
							class="m-auto h-6 w-6 text-gray-700 dark:text-white"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								d="M3.75 13.5l10.5-11.25L12 10.5h8.25L9.75 21.75 12 13.5H3.75z"
							/>
						</svg>
					</Feature>
				</div>
			</div>
		</div>
	</Container>
</div>
