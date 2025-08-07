<script lang="ts">
  export let title: string;

  export let date: string;

  export let technologies: string[] = [];

  export let links: [string, string][] = [];
</script>

<article class="group text-left">
  <div class="flex justify-between sm:items-center flex-col sm:flex-row">
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
    <h2>{date}</h2>
  </div>

  <slot />

  {#if technologies.length}
    <p>
      Technologies:
    </p>
    <ul class="list-disc ml-3">
      {#each technologies as tech}
        <li>{tech}</li>
      {/each}
    </ul>
  {/if}

  {#if links.length}
    <p>
      More about this project:
    </p>
    <ul class="list-disc ml-3">
      {#each links as [href, label]}
        <li>
          <a href={href} target="_blank" rel="noopener noreferrer">
            {label}
          </a>
        </li>
      {/each}
    </ul>
  {/if}
  
</article>