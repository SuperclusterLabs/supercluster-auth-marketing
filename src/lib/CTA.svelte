<script lang="ts">
	import { onMount } from 'svelte';
	import Container from './Container.svelte';
	import Button from './Button.svelte';

	const activityText = ['building', 'writing', 'podcasting', 'developing', 'designing'];
	let activityCounter: number = 0;
	let currentActivity: string = activityText[0];

	function changeActivityText() {
		activityCounter++;
		if (activityCounter >= activityText.length) {
			activityCounter = 0;
		}
		currentActivity = activityText[activityCounter];
	}

	onMount(() => {
		setInterval(changeActivityText, 2000);
	});
</script>

<div class="bg-planetYellow py-10 px-5 md:p-20 mx-auto mt-28">
	<Container>
		<h1 class="text-2xl md:text-4xl mb-10 leading-relaxed">
			We’ve built an access management platform based on engagement, not identity.<br /><br />
			<span class="font-bold"
				>So your community can focus on
				<span class="my-4 underline underline-offset-4">{currentActivity}</span>.
			</span>
		</h1>
		<Button>Get early access</Button>
	</Container>
</div>
