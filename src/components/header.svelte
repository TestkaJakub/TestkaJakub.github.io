<header class="pt-6 pb-12">
  <div class="mx-auto px-10 sm:px-20 flex flex-row justify-between gap-5 place-items-start ">
    <div class="flex flex-col sm:flex-row sm:gap-5 gap-2 sm:place-items-center place-self-center">
      <h1 class="text-2xl font-semibold">JakubT.Portfolio</h1>
      <nav>
        <ul class="flex space-x-4 list-none">
          <li><a href="/">Home</a></li>
          <li><a href="/about">About</a></li>
          <li><a href="/projects">Projects</a></li>
        </ul>
      </nav>
    </div>
    <ThemeToggle/>
  </div>
</header>

<script lang="ts">
  import ThemeToggle from "./theme-toggle.svelte";
</script>