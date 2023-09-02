<script>
	import { base } from '$app/paths';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte beeq" />
</svelte:head>

<section>
	<h1>Hello Bee-q</h1>
	<bq-button>hello world</bq-button>
	<bq-button appearance="link" href="{base}/about">About page</bq-button>
</section>

<style>
</style>
