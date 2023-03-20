<script lang="ts">
	import Container from './Container.svelte';
	import SCLogoBW from '$lib/assets/SC-Logotype-BW.svg';
</script>

<header>
	<nav
		class="absolute z-10 w-full border-b border-black/5 dark:border-white/5 lg:border-transparent"
	>
		<Container>
			<div
				class="relative flex flex-wrap items-center justify-between gap-6 py-2 md:gap-0 md:py-6 px-8 my-6 bg-white drop-shadow-md rounded-full"
			>
				<div class="relative z-20 flex w-full justify-between md:px-0 lg:w-max">
					<a href="#home" aria-label="logo" class="flex items-center space-x-2">
						<img class="w-[280px]" src={SCLogoBW} alt="Supercluster Logo" />
					</a>
				</div>
			</div>
		</Container>
	</nav>
</header>
