<script lang="ts">
	import Card from './Card.svelte';
	import NotionImage from '$lib/assets/Notion.png';
	import GoogleDocImage from '$lib/assets/GoogleDoc.png';
</script>

<div class="mb-20 md:mb-32">
	<h3 class="text-2xl font-bold text-gray-900 dark:text-white md:w-2/3 md:text-3xl lg:text-4xl">
		Some simple use cases
	</h3>
	<div class="relative mt-12 grid gap-6 sm:grid-cols-2 lg:grid-cols-2">
		<Card>
			<div>
				<img src={NotionImage} alt="safety icon illustration" height="512" width="512" />
				<h4 class="text-xl font-semibold text-gray-900 dark:text-white">
					Gate your Notion workspace(s) using NFTs
				</h4>
				<p class="mt-3 text-gray-600 dark:text-gray-400">
					Send NFTs to your premium members and give them access to exclusive content on Notion
				</p>
			</div>
		</Card>
		<Card>
			<div>
				<img src={GoogleDocImage} alt="safety icon illustration" height="512" width="512" />
				<h4 class="text-xl font-semibold text-gray-900 dark:text-white">
					Only allow members who recently voted access to your Google Docs content
				</h4>
				<p class="mt-3 text-gray-600 dark:text-gray-400">
					Make sure only those who have voted on a Snapshot proposal within the last month have
					access to your upcoming proposal content on Google Drive.
				</p>
			</div>
		</Card>
	</div>
</div>
