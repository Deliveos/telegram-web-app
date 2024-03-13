<script>
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
    import Item from '$lib/components/Item.svelte';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<h1>Create your first character</h1>
	<div class="character-editor">
		<Item><div class="character">1</div></Item>
		<div class="character-editor_types">
			<Item><div class="card"><Counter/></div></Item>
			<Item><div class="card"></div></Item>
			<Item><div class="card"></div></Item>
			<Item><div class="card"></div></Item>
		</div>
	</div>
</section>

<style>
	section {
		background-color: var(--tg-theme-bg-color);
		color: var(--tg-theme-text-color);
		width: 100vw;
		height: 100vh;
		padding-right: 10%;
		padding-left: 10%;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
	}

	.card {
		width: 20vw;
		height: 20vw;
	}

	.character {
		width: 60vw;
	}

	.character-editor {
		padding-left: 10%;
		padding-right: 10%;
		display: flex;
		gap: 20px;
	}

	.character-editor_types {
		display: flex;
		gap: 20px;
		flex-direction: column;
	}
</style>
