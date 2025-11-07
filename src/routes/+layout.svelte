<script lang="ts">
    import '../app.css';
    import '$lib/styles/landing.css';
    import { onMount } from 'svelte';
    import favicon from '$lib/assets/favicon.svg';

    let { children } = $props();

    onMount(() => {
        const root = document.documentElement;
        const body = document.body;

        root.classList.add('dark');
        body.style.backgroundColor = '#0D0D0F';
        body.style.color = '#ffffff';
        body.style.fontFamily = 'Inter, sans-serif';

        return () => {
            root.classList.remove('dark');
            body.style.removeProperty('background-color');
            body.style.removeProperty('color');
            body.style.removeProperty('font-family');
        };
    });
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous" />
    <link
        rel="stylesheet"
        href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&display=swap"
    />
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined" />
</svelte:head>

{@render children()}
