<script lang="ts">
	import Container from './Container.svelte';
	import SCLogoBW from '$lib/assets/SC-Logotype-BW.svg';
	import Button from './Button.svelte';
</script>

<header>
	<nav>
		<Container>
			<div
				class="relative flex flex-wrap items-center justify-center sm:justify-between py-6 px-8 mt-6 bg-transparent md:bg-white drop-shadow-xl rounded-full"
			>
				<div class="relative flex justify-between md:px-0">
					<a href="/" aria-label="logo" class="flex items-center">
						<img class="w-[280px]" src={SCLogoBW} alt="Supercluster Logo" />
					</a>
				</div>
				<div class="hidden sm:block">
					<Button>Get early access</Button>
				</div>
			</div>
		</Container>
	</nav>
</header>
