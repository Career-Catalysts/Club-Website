<script lang="ts">
	import '../app.postcss'
	import Header from './Header.svelte'
</script>

	<div id="header">
		<Header />
	</div>

	<div id="main-section">
		<main
			class="flex flex-col justify-center items-center"
		>
			<slot />

			<!-- <Footer /> -->
		</main>
	</div>

<style>
	:global(body) {
		margin: 0;
	}

	#header {
		text-align: center;
		color: #fff;
		width: 100%;
		background: rgb(8, 12, 21);
	}

	#main-section {
		text-align: center;
		color: #fff;
		width: 100%;

		/* height: 90vh; */
		background: linear-gradient(
			180deg,
			rgba(13, 19, 32, 1) 0%,
			rgba(8, 12, 21, 1) 100%
		);
	}
</style>
