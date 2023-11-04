<script lang="ts">
	import '../app.postcss'
	import { ModeWatcher } from 'mode-watcher'
	import Header from './Header.svelte'
</script>

<ModeWatcher />

<Header />

<main class='flex justify-center items-center bg-yellow-200 h-[70vh] pb-11'>
	<slot />

	<!-- <Footer /> -->
</main>
