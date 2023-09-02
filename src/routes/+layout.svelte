<script>
	import './styles.css';
	import { applyPolyfills, defineCustomElements } from '@bee-q/core/dist/loader';

	let ready = false;

	applyPolyfills().then(() => {
		defineCustomElements();
		ready = true;
	});
</script>

{#if ready}
	<div class="app">
		<main>
			<slot />
		</main>
	</div>
{/if}
