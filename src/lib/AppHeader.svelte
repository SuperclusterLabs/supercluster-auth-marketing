<script lang="ts">
	import Container from './Container.svelte';
	import SCLogoBW from '$lib/assets/SC-Logotype-BW.svg';
</script>

<header>
	<nav
		class="absolute z-10 w-full border-b border-black/5 dark:border-white/5 lg:border-transparent"
	>
		<Container>
			<div class="relative flex flex-wrap items-center justify-between gap-6 py-2 md:gap-0 md:py-4">
				<div class="relative z-20 flex w-full justify-between md:px-0 lg:w-max">
					<a href="#home" aria-label="logo" class="flex items-center space-x-2">
						<img class="w-[280px]" src={SCLogoBW} alt="Supercluster Logo" />
					</a>
				</div>

				<div class="hidden sm:visible lg:mt-0">
					<a
						href="https://form.waitlistpanda.com/go/L0zfvXH00hvIG9DSTLUw"
						target="_blank"
						rel="noreferrer"
						class="relative flex h-9 w-full items-center justify-center px-4 before:absolute before:inset-0 before:rounded-full before:bg-primary before:transition before:duration-300 hover:before:scale-105 active:duration-75 active:before:scale-95 sm:w-max"
					>
						<span class="relative font-semibold text-white">Sign up</span>
					</a>
				</div>
			</div>
		</Container>
	</nav>
</header>
