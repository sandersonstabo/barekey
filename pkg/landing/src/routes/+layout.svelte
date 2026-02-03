<script lang="ts">
	import './layout.css';
	import "@fontsource/google-sans-flex";

	import favicon from '$lib/assets/favicon.svg';
	import { ModeWatcher } from 'mode-watcher';

	let { children } = $props();
</script>

<svelte:head>
	<link href="https://fonts.cdnfonts.com/css/pp-neue-montreal" rel="stylesheet">
	<link rel="icon" href={favicon} />
</svelte:head>

<ModeWatcher />
{@render children()}
