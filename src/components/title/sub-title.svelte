<script>
  export let index = null;
</script>

<div class="sub-title">
  {index !== null ? index + '. ' : '▷'}
  <slot />
</div>
