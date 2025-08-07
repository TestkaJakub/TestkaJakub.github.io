<script lang="ts">
  import { onMount } from 'svelte';

  import MoonIcon from '$lib/assets/moon-svgrepo-com.svg';
  import SunIcon from '$lib/assets/sun-svgrepo-com.svg';

  type Theme = 'light' | 'dark';

  let theme: Theme = 'light';

  onMount(() => {
    const saved = localStorage.getItem('theme') as Theme | null;
    const prefersDark = window
      .matchMedia('(prefers-color-scheme: dark)')
      .matches;

    theme = saved ?? (prefersDark ? 'dark' : 'light');
    document.documentElement.setAttribute('data-theme', theme);
  });

  function toggleTheme(): void {
    theme = theme === 'dark' ? 'light' : 'dark';
    document.documentElement.setAttribute('data-theme', theme);
    localStorage.setItem('theme', theme);
  }
</script>

<button
  aria-label="Toggle dark mode"
  class="p-2 rounded hover:outline-none transition"
  on:click={toggleTheme}
>
  {#if theme === 'dark'}
    <img
      src={SunIcon}
      alt="Switch to light mode"
      class="w-5 h-5"
    />
  {:else}
    <img
      src={MoonIcon}
      alt="Switch to dark mode"
      class="w-5 h-5"
    />
  {/if}
</button>