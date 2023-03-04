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
				<input
					aria-hidden="true"
					type="checkbox"
					name="toggle_nav"
					id="toggle_nav"
					class="peer hidden"
				/>
				<div class="relative z-20 flex w-full justify-between md:px-0 lg:w-max">
					<a href="#home" aria-label="logo" class="flex items-center space-x-2">
						<img class="w-[350px]" src={SCLogoBW} alt="Supercluster Logo" />
					</a>

					<div class="relative flex max-h-10 items-center lg:hidden">
						<label
							role="button"
							for="toggle_nav"
							aria-label="humburger"
							id="hamburger"
							class="relative -mr-6 p-6"
						>
							<div
								aria-hidden="true"
								id="line"
								class="m-auto h-0.5 w-5 rounded bg-sky-900 transition duration-300 dark:bg-gray-300"
							/>
							<div
								aria-hidden="true"
								id="line2"
								class="m-auto mt-2 h-0.5 w-5 rounded bg-sky-900 transition duration-300 dark:bg-gray-300"
							/>
						</label>
					</div>
				</div>

				<div class="mt-12 lg:mt-0">
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

<style>
	#toggle_nav:checked ~ div #hamburger #line {
		@apply translate-y-1.5 rotate-45;
	}

	#toggle_nav:checked ~ div #hamburger #line2 {
		@apply -translate-y-1 -rotate-45;
	}
</style>
