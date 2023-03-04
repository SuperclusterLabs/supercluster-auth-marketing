<script lang="ts">
	import '../app.css';

	import HeroSection from '$lib/HeroSection.svelte';
	import Features from '$lib/Features.svelte';
	import AppHeader from '$lib/AppHeader.svelte';
	import Solution from '$lib/Solution.svelte';
	import AppFooter from '$lib/AppFooter.svelte';
</script>

<main>
	<AppHeader />
	<HeroSection />
	<Features />
	<Solution />
	<AppFooter />
</main>
