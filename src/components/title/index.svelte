<script>
  export let title = "";
  export let index = null;
</script>

<div class="title">
  {#if title}
    <p class="title__header">{index !== null ? index + '. ' : '▶'} {title}</p>
    <slot />
  {:else}
    <p class="title__header">
      {index !== null ? index + '. ' : '▶'}
      <slot />
    </p>
  {/if}

</div>
