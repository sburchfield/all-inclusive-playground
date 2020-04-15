<script>
  export let className = false;
</script>

<div class={"color-card white " + className}>
  <slot name="header"></slot>
  <slot></slot>
</div>

<style>
  .color-card{
    height: 18em;
    padding: 2em 0 0 0;
  }
</style>
