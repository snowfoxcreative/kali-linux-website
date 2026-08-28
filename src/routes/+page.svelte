<!--
The default page of the website. It displays the boot screen and directs the user to
/desktop or /terminal depending on what they choose.
-->

<script lang="ts">
import BootScreen from "$lib/components/BootScreen.svelte";

import "../app.css";
</script>

<main>
  <BootScreen />
</main>

<style>
main {
  width: 100vw;
  height: 100vh;
}
</style>
