<script lang="ts">
  import "../app.postcss";
  import { ModeWatcher } from "mode-watcher";
  import Header from "./Header.svelte";
</script>

<ModeWatcher />

<Header />

<main class='flex justify-center screen items-center h-[70vh] pb-11'>
  <slot />

  <!-- <Footer /> -->
</main>

<style>
	.screen {
  margin: 0 auto;
  width: vh;
  height: vw;

  background: rgb(193,193,193);
  background: radial-gradient(circle at 42% 5%, rgba(123,123,123,1) 0%, rgba(50,50,50,1) 26%, rgba(0,0,0,1) 52%);
}
</style>
