<script lang="ts">
  export let count: number
</script>

<style lang="scss">
  $background-color: #666666;
  $color: #f0f0f0;
  .number {
    background-color: $background-color;
    color: $color;
    padding: 2px 5px;
    border-radius: 3px;
    width: 18.25px;
  }
</style>

<div class="number">+{count}</div>
