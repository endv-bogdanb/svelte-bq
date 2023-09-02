<script lang="ts">
	import './styles.css';

	// @ts-expect-error loaders not working properly
	import { applyPolyfills, defineCustomElements } from '@bee-q/core/dist/loader/index.cjs';

	let ready = false;

	void (async function load(): Promise<void> {
		await applyPolyfills();
		defineCustomElements();
		ready = true;
	})();
</script>

{#if ready}
	<div class="app">
		<main>
			<slot />
		</main>
	</div>
{/if}
