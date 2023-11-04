<script lang="ts">
	import '../app.postcss'
	import { ModeWatcher } from 'mode-watcher'
	import Header from './Header.svelte'
</script>

<ModeWatcher />

<Header />

<main class='flex justify-center items-center text-l'>
	<slot />

	<!-- <Footer /> -->
</main>
