<script>
  export let icon = ''
  export let title = ''
</script>
<div class="info__item">
  <i class={'i ' + icon}></i>
  <p class="info__item-content" title={title}><slot></slot></p>
</div>