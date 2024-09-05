<script>
	import Todos from '$lib/components/Todos.svelte';
	import ThemeChanger from '$lib/components/ThemeChanger.svelte';
</script>

<svelte:head>
	<title>TodoList</title>
	<meta name="description" content="Demo project making a todolist" />
</svelte:head>
<div class="flex items-center justify-between bg-base-100 p-4">
	<div class="flex-1 text-center">
		<h1 class="italic font-mono text-3xl">Todos</h1>
	</div>
	<ThemeChanger />
</div>
<Todos />

<style lang="postcss">
	:global(html) {
		background-color: theme(colors.gray.100);
	}
</style>
