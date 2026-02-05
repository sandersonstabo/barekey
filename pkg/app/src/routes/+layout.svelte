<script lang="ts">
	import './layout.css';
	import "@fontsource/google-sans-flex";

	import { IconMoonFilled, IconSunFilled } from "@tabler/icons-svelte";

	import favicon from '$lib/assets/favicon.svg';
	import { mode, ModeWatcher, toggleMode } from 'mode-watcher';
    import { Button } from '$lib/components/ui/button';

	let { children } = $props();
</script>

<svelte:head>
	<link href="https://fonts.cdnfonts.com/css/pp-neue-montreal" rel="stylesheet">
	<link rel="icon" href={favicon} />
</svelte:head>

<ModeWatcher />
{@render children()}

<Button class="absolute top-4 right-4" onclick={toggleMode}>
	{#if mode.current === "dark"}
		<IconSunFilled />
	{:else}
		<IconMoonFilled />
	{/if}
</Button>