<script>
import { base } from '$app/paths';

	
</script>
<svelte:head>
       <link rel="stylesheet" href="{base}/bootstrap.min.css"> 
       <link rel="stylesheet" href="{base}/w3.css">
     </svelte:head>

<div class="app">
	<h1>hello i m the best</h1>
	<button class="btn btn-primary">click me</button>

	<main><slot /></main>

	<h2>Hello u know me </h2>	
	
</div>

<style>
	
</style>
