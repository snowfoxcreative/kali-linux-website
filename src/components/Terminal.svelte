<script lang="ts">
  import img from "$lib/assets/utilities-terminal.png";
  let dir = $state("~");
</script>

<div class="terminal">
  <div class="terminal-header">
    <div class="terminal-header__title-bar">
      <img src={img} alt="" />
      kali@kali: {dir}
      <div class="terminal-header__title-bar__window-control">
        <button></button>
        <button></button>
        <button></button>
      </div>
    </div>
    <div class="terminal-header__menu-bar">

    </div>
  </div>
  <div class="terminal-body">

  </div>
</div>

<style>
  .terminal {
    display: flex;
    flex-direction: column;
    width: 600px;
    height: 400px;
  }

  .terminal-header {
    display: flex;
    flex-direction: column;
    width: 100%;
  }

  .terminal-header__title-bar {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
  }

  .terminal-header__title-bar__window-control {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    gap: 10px;
  }

  .terminal-header__menu-bar {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: flex-start;
    gap: 16px;
  }

  .terminal-body {
    width: 100%;
    overflow-y: scroll;
  }
</style>
