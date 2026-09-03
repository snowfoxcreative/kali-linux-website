<!-- 
Screen.svelte

Screen in desktop GUI
-->

<script lang="ts">
import screenImg from "$lib/assets/kali-cubism.jpg";
</script>

<div class="screen">
  <enhanced:img
    class="screen-img"
    src={screenImg}
    alt="Abstract dark blue and gray cubist geometric background featuring the central Kali Linux dragon logo rendered in a fractured, low-poly style."
  />
</div>

<style>
.screen {
  width: 100vw;
  display: grid;
  flex: 1 0 0;
  position: relative;
}

.screen-img {
  width: 100%;
  height: 100%;
  position: absolute;
  object-fit: cover;
  z-index: 0;
}
</style>
