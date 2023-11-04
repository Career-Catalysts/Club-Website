<script lang="ts">
	import '../app.postcss'
	import { ModeWatcher } from 'mode-watcher'
	import Header from './Header.svelte'
  import { mode } from 'mode-watcher'

	let theme_mode = ''
	mode.subscribe((m) => (theme_mode = m))
  console.log(theme_mode);
  $: theme_mode_class = (theme_mode === 'dark' ? 'screen-dark' : 'screen-light');
  
  
</script>

<ModeWatcher />

<Header />

<main class="flex justify-center items-center h-[70vh] pb-11" class:theme_mode_class>
	<slot />

	<!-- <Footer /> -->
</main>

<style>
	.dark {
		margin: 0 auto;
		width: vh;
		height: vw;

		background: radial-gradient(
			circle at 42% 5%,
			rgba(123, 123, 123, 1) 0%,
			rgba(50, 50, 50, 1) 26%,
			rgba(0, 0, 0, 1) 52%
		);
	}
	.light {
		margin: 0 auto;
		width: vh;
		height: vw;

		background: radial-gradient(
			circle at 42% 5%,
			rgba(132, 132, 132, 1) 0%,
			rgba(205, 205, 205, 1) 26%,
			rgba(255, 255, 255, 1) 52%
		);
	}
</style>
