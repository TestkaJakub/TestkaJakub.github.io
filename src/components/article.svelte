<script lang="ts">
  export let title: string;
</script>

<article class="group text-left">
  <h2
    class="
      flex
      items-center
      text-2xl

      before:content-['✦']
      before:inline-block
      before:mr-2

      before:origin-center
      before:transition
      before:duration-[1000ms]
      before:ease-in-out

      before:text-[var(--secondary)]
      group-hover:before:text-[var(--primary)]
      group-hover:before:rotate-[320deg]
    "
  >
    {title}
  </h2>

  <slot />
</article>