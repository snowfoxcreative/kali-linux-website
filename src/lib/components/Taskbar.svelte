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
        src={menuImg}
        alt="Kali Linux dragon logo"
      />
    </button>
    <div class="taskbar-divider"></div>
  </div>
  <div></div>
  <div></div>
  <div class="taskbar-main-menu">
  </div>
</div>

<style>
.taskbar {
  width: 100vw;
  height: 2rem;
  display: flex;
  flex-direction: row;
  align-items: center;
  position: relative;
  background-color: #223647;
  border-bottom: 2px solid #0e0f12;
}

.taskbar-left {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 0.25rem;
}

.taskbar-btn {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 2rem;
  height: 2rem;
  padding: 0.25rem;
  background: none;
  border: none;
  outline: none;
}

.taskbar-img {
  width: 100%;
  height: 100%;
  object-fit: contain;
}

.taskbar-divider {
  width: 1.5px;
  height: 1.25rem;
  background-color: #8f98a0;
}

.taskbar-main-menu {
  display: flex;
  position: absolute;
}
</style>
