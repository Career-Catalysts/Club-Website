<script lang="ts">
	import '../app.postcss'
	import { ModeWatcher } from 'mode-watcher'
	import Header from './Header.svelte'
	import { mode } from 'mode-watcher'
	import App from '$lib/components/App.svelte'

	let theme_mode = 'dark'
	mode.subscribe((m) => (theme_mode = m))
	$: if (theme_mode == 'light') {
		// 	document.body.classList.add('light')
		// } else {
		// 	document.body.classList.remove('light')
	}
</script>

<div id="container">
	<ModeWatcher />

	<!-- threejs scene background -->
	<App />

	<div id="header">
		<Header />
	</div>

	<div id="main-section">
		<main
			class="flex flex-col {`${
				theme_mode == 'light' ? 'sclight' : 'scdark'
			}`} justify-center items-center"
		>
			<slot />

			<!-- <Footer /> -->
		</main>
	</div>
</div>

<style>
	:global(body) {
		margin: 0;
	}

	#container {
		width: 100vw;
		height: 200vh;
		background: linear-gradient(
			180deg,
			rgba(13, 19, 32, 1) 0%,
			rgba(8, 12, 21, 1) 100%
		);
	}

	#header {
		position: absolute;
		text-align: center;
		color: #fff;
		width: 100%;
		height: 10vh;
		top: 0;
		background-color: #0d1320;
		/* z-index: -1 */
	}

	#main-section {
		position: absolute;
		text-align: center;
		color: #fff;
		width: 100%;
		height: 90vh;
		bottom: 0;
		/* z-index: -1 */
	}
</style>
