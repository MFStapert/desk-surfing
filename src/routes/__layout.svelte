<script>
	import Topbar from '$lib/components/Topbar.svelte';
	import Pageheader from '$lib/components/Pageheader.svelte';
	import Navigation from '$lib/components/Navigation.svelte';
	import '../styles/app.css';
</script>

<header class="topbar">
	<Topbar />
</header>

<nav class="navigation">
	<Navigation />
</nav>

<main class="main">
	<slot />
</main>
