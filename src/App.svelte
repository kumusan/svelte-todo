<script>
	import Greeting from './Greeting.svelte'
	import Card from './Card.svelte'

	let name = ''
	let checked = false
	const arr = [
		{name: 'te1'},
		{name: 'te2'},
		{name: 'te3'}
	]
</script>

<main>
  <Card>
		<Greeting username="kfsdjklfj" />
	</Card>

	<input placeholder="your name" bind:value={name}>
	<div>hee {name}</div>

	<input type="checkbox" bind:checked={checked}>
	{#if checked}
		<div>okokokoko</div>
	{:else}
		<div>nonono</div>
	{/if}
	
	{#each arr as a}
		<div>{a.name}</div>
  {/each}
</main>

<style>
</style>
