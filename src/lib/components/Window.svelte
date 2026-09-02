<!-- 
Window.svelte

Window that opens after a user clicks on a desktop app.
-->

<script lang="ts"></script>

<div class="window">
  <div class="window-top-bar"></div>
  <div class="window-content"></div>
</div>

<style>
.window {
  display: flex;
  flex-direction: column;
}

.window-top-bar {
  border: 1px solid red;
}

.window-content {
  border: 1px solid red;
}
</style>
