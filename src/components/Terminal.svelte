<script lang="ts">
  import img from "$lib/assets/utilities-terminal.png";

  const username = "zulaikha";
  const hostname = "portfolio";
  const bottomPrompt = "└─$ ";

  let dir = $state("~");
  let topPrompt = $derived(`┌──(${username}㉿${hostname})-[${dir}]`);
  let history = $state([]);

  function minimize() {
    
  }

  function restore() {

  }

  function close() {

  }
</script>

<div class="terminal">
  <div class="terminal-header">
    <div class="terminal-header__title-bar">
      <img src={img} alt="" />
      {username}@{hostname}: {dir}
      <div class="terminal-header__title-bar__window-control">
        <button
          aria-label="Minimize"
          class="terminal-header__title-bar__button"
          onclick={minimize}
        ></button>
        <button
          aria-label="Restore"
          class="terminal-header__title-bar__button"
          onclick={restore}
        ></button>
        <button
          aria-label="Close"
          class="terminal__title-bar__button"
          onclick={close}
        ></button>
      </div>
    </div>
    <div class="terminal-header__menu-bar">
      <div class="terminal-header__menu-item">
        File
      </div>
      <div class="terminal-header__menu-item">
        Actions
      </div>
      <div class="terminal-header__menu-item">
        Edit
      </div>
      <div class="terminal-header__menu-item">
        View
      </div>
      <div class="terminal-header__menu-item">
        Help
      </div>
    </div>
  </div>
  <div class="terminal-body">
    <textarea class="terminal-body__textarea"></textarea>
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

  .terminal-header__title-bar__button {
    border-radius: 50%;
    aspect-ratio: 1;
  }

  .terminal-header__menu-bar {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: flex-start;
    gap: 16px;
  }

  .terminal-header__menu-item {
    padding: 0 10px;
  }

  .terminal-body {
    width: 100%;
    overflow-y: scroll;
  }

  .terminal-body__textarea {
    width: 100%;
    height: 100%;
    line-height: 1;
  }
</style>
