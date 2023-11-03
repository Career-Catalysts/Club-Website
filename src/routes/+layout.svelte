<script lang="ts">
	import '../app.postcss'
	import { ModeWatcher } from 'mode-watcher'
	import Header from './Header.svelte'
</script>

<ModeWatcher />

<main class='m-6'>
	<Header />

	<slot />

	<!-- <Footer /> -->
</main>
