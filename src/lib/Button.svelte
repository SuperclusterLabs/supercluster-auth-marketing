<script lang="ts">
	export let label: string = '';
	export let type: string = '';
	export let emphasis: string = '';
	export let to: string = '';
</script>

<a
	href={to}
	class={emphasis == 'primary'
		? 'before:bg-primary'
		: 'before:border before:border-transparent before:bg-primary/10 dark:before:border-gray-700 dark:before:bg-gray-800'}
	{type}
>
	<span class={emphasis == 'primary' ? 'text-white' : 'text-primary dark:text-white'}>
		{label}
	</span>
</a>

<!-- <style>
	a,
	button {
		@apply relative flex h-11 w-max items-center justify-center px-5 before:absolute before:inset-0 before:rounded-full before:transition before:duration-300 hover:before:scale-105 active:duration-75 active:before:scale-95;
	}
	span {
		@apply relative w-max text-base font-semibold;
	}
</style> -->
