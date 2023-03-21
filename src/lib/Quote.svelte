<script lang="ts">
	import Container from '$lib/Container.svelte';
	import quoteImage from '$lib/assets/quotation.png';
</script>

<Container>
	<div
		class="bg-[url('./assets/quotation.png')] bg-white relative p-14 shadow-xl rounded-3xl mt-20"
	>
		<p class="text-lg md:text-2xl leading-relaxed">
			"We're constantly struggling with getting file access shared anonymously through web2 apps...
			We spend an incredible amount of time trying to manage those platforms.<br /><br />
			<span class="font-bold"
				>The access control features from Supercluster would save our team at least 10 hours a week…
				<span class="text-planetYellow">Stoked that this giant issue is now being solved."</span
				></span
			>
		</p>
		<p class="mt-10 text-lg md:text-2xl italic">
			OrnellaWeb3, <span class="font-bold">BanklessDAO</span>
		</p>
		<img alt="Quote background" class="top-[30px] left-[20px] absolute" src={quoteImage} />
	</div>
</Container>
