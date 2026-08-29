<!--
BootScreen.svelte

This is the screen that displays when the site first loads. It allows the user to select whether
to view the site in normal mode (like a regular site) or as a desktop GUI.
-->

<script lang="ts">
import { resolve } from "$app/paths";

// Auto-route to /desktop if user doesn't choose in a certain amount of time
</script>

<div class="container">
  <span class="text2">
    Hello and welcome to Zulaikha's website!
  </span>
  <span class="text2">
    Select how you would like to experience it.
  </span>
  <div class="box">
    <a class="text highlight" href={resolve("/desktop")}>
      Kali Linux (Desktop GUI)
    </a>
    <a class="text" href={resolve("/terminal")}>
      Terminal (Text GUI)
    </a>
  </div>
  <span class="text2">
    Use the ...
    Happy exploring!
  </span>
  <span class="text2">
    - Zulaikha
  </span>
</div>

<style>
* {
  font-family: var(--font-boot-terminal);
}

.container {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  background-color: #31001d;
}

.text {
  color: #fefefe;
}

.text2 {
  color: #d5d5d5;
}

.box {
  border: 2px solid #fefefe;
}

.highlight {
  color: black;
  background-color: #d5d5d5;
}

/* width >= 400px */
@media (min-width: 25rem) {
}

/* width >= 640px */
@media (min-width: 40rem) {
}

/* width >= 768px */
@media (min-width: 48rem) {
}

/* width >= 1024px */
@media (min-width: 64rem) {
}

/* width >= 1280px */
@media (min-width: 80rem) {
}

/* width >= 1536px */
@media (min-width: 96rem) {
}

/* width >= 1920px */
@media (min-width: 120rem) {
}
</style>
