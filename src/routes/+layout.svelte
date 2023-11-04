<script lang="ts">
  import "../app.postcss";
  import { ModeWatcher } from "mode-watcher";
  import Header from "./Header.svelte";
</script>

<ModeWatcher />

<Header />

<main>
  <slot />

  <!-- <Footer /> -->
</main>
