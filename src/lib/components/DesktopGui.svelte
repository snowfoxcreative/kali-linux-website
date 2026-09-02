<!--
DesktopGui.svelte

The component emulating the desktop GUI if the user selects to view the website
in desktop GUI mode.
-->

<script lang="ts">
import Screen from "./Screen.svelte";
import Taskbar from "./Taskbar.svelte";

const asciiName = "\
 _____     _       _ _    _           \
|__  /   _| | __ _(_) | _| |__   __ _ \
  / / | | | |/ _` | | |/ / '_ \ / _` |\
 / /| |_| | | (_| | |   <| | | | (_| |\
/____\__,_|_|\__,_|_|_|\_\_| |_|\__,_|\
".trim();


</script>

<div class="container">
  <Taskbar />
  <Screen />
</div>

<style>
.container {
  width: 100vw;
  height: 100vh;
}
</style>
