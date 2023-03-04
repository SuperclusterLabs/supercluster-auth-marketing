<script lang="ts">
	import Container from './Container.svelte';
	import SCLogoBW from '$lib/assets/SC-Logotype-BW.svg';
	import DiscordSVG from '$lib/assets/discord.svg';
	import TwitterSVG from '$lib/assets/twitter.svg';
</script>

<footer class="bg-gradient-to-b from-transparent to-gray-100 pb-12 dark:to-gray-900">
	<Container>
		<a href="#home" aria-label="logo" class="flex items-center justify-center space-x-2">
			<a href="#home" aria-label="logo" class="flex items-center space-x-2">
				<img class="w-[350px]" src={SCLogoBW} alt="Supercluster Logo" />
			</a>
		</a>
		<div class="m-auto mt-4 flex w-max items-center justify-between space-x-4 text-gray-500">
			<a
				class="duration-300 hover:text-gray-600 dark:hover:text-white"
				href="https://discord.gg/shKeHySU"
				title="discord"
				target="blank"
				aria-label="discord"
			>
				<img class="w-[35px]" src={DiscordSVG} alt="Discord Logo" />
			</a>
			<a
				class="duration-300 hover:text-gray-600 dark:hover:text-white"
				href="https://twitter.com/superclusterdev"
				title="twitter"
				target="blank"
				aria-label="twitter"
			>
				<img class="w-[35px]" src={TwitterSVG} alt="Twitter Logo" />
			</a>
		</div>

		<div class="mt-12 text-center">
			<span class="text-sm tracking-wide text-gray-500"
				>Copyright © Supercluster Labs 2023 | All rights reserved</span
			>
		</div>
	</Container>
</footer>
