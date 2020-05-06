<script>
	import Home from './Home.svelte';
	import Router from 'svelte-spa-router'
	import Add from './components/Add.svelte'

	const routes = {
		'/': Home,
		'/add': Add,
		'*': Home,
	}
</script>

<main>
	<Router routes={routes}></Router>
</main>

<style>
	main {
		background-color: rgb(255, 251, 246);
		padding: 2em;
		width: 100%;
		height: 100%;
		overflow-y: auto;
	}
</style>