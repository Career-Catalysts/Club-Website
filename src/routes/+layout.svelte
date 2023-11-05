<script lang="ts">
	import '../app.postcss'
	import { ModeWatcher } from 'mode-watcher'
	import Header from './Header.svelte'
  import { mode } from 'mode-watcher'

	let theme_mode = 'dark'
	mode.subscribe((m) => (theme_mode = m))
</script>

<ModeWatcher />

<Header />

<main class="flex flex-col {`${theme_mode == 'light' ? 'sclight' : 'scdark'}`} ">
	<slot />

	<!-- <Footer /> -->
</main>

<style>
	.scdark {
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
	.sclight {
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
