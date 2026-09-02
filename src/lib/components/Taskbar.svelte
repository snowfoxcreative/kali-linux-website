<!-- 
Taskbar.svelte

Taskbar in desktop GUI
-->

<script lang="ts">
import menuImg from "$lib/assets/kali-panel-menu.svg";

const openMainMenu = () => {};
</script>

<div class="taskbar">
  <div class="taskbar-left">
    <button class="taskbar-btn" onclick={openMainMenu} aria-label="Open main menu">
      <enhanced:img
        class="taskbar-img"
        src="/kali-panel-menu.svg"
        alt="Kali Linux dragon logo"
      />
    </button>
  </div>
  <div></div>
  <div></div>
</div>

<style>
.taskbar {
  width: 100vw;
  display: flex;
}

.taskbar-left {
  display: flex;
  flex-direction: row;
}
</style>
