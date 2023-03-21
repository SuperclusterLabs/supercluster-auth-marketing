<script lang="ts">
	import '../app.css';

	import HeroSection from '$lib/HeroSection.svelte';
	import Features from '$lib/Features.svelte';
	import AppHeader from '$lib/AppHeader.svelte';
	import AppFooter from '$lib/AppFooter.svelte';
	import Supporters from '$lib/Supporters.svelte';
	import Circles from '$lib/Circles.svelte';
	import Quote from '$lib/Quote.svelte';
	import CTA from '$lib/CTA.svelte';
</script>

<main class="bg-backgroundColor">
	<Circles />
	<AppHeader />
	<HeroSection />
	<Supporters />
	<Features />
	<Quote />
	<CTA />
	<AppFooter />
</main>
