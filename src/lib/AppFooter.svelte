<script lang="ts">
	import Container from './Container.svelte';
	import SCLogoColor from '$lib/assets/SC-Logotype-Color.svg';
	import DiscordSVG from '$lib/assets/discord.svg';
	import TwitterSVG from '$lib/assets/twitter.svg';
	import LinkedinSVG from '$lib/assets/linkedin.svg';
</script>

<footer class="bg-deepBlue w-full">
	<Container>
		<div class="flex flex-row justify-between py-6">
			<a href="#home" aria-label="logo" class="flex items-center justify-center space-x-2">
				<a href="#home" aria-label="logo" class="flex items-center space-x-2">
					<img class="w-[215px]" src={SCLogoColor} alt="Supercluster Logo" />
				</a>
			</a>
			<div class="flex flex-row gap-4">
				<a
					class="duration-300 hover:text-gray-600 dark:hover:text-white"
					href="https://twitter.com/superclusterdev"
					title="twitter"
					target="blank"
					aria-label="twitter"
				>
					<img class="w-[35px]" src={TwitterSVG} alt="Twitter Logo" />
				</a>
				<a
					class="duration-300 hover:text-gray-600 dark:hover:text-white"
					href="https://discord.gg/KxRPj43aPT"
					title="discord"
					target="blank"
					aria-label="discord"
				>
					<img class="w-[35px]" src={DiscordSVG} alt="Discord Logo" />
				</a>
				<a
					class="duration-300 hover:text-gray-600 dark:hover:text-white"
					href="https://www.linkedin.com/company/supercluster-labs/"
					title="linkedin"
					target="blank"
					aria-label="linkedin"
				>
					<img class="w-[35px]" src={LinkedinSVG} alt="LinkedIn Logo" />
				</a>
			</div>
		</div>
	</Container>
</footer>
