<script lang="ts">
  export let isOverflowing = false
  export let recipients: string[]
  let divWidth = recipients.length > 1 ? 'calc(100% - 18px)' : ''
</script>

<style>
  .recipents {
    min-width: 0;
  }
</style>

<!--
@component
Receives a `recipients` prop as an array of strings 
and renders string and possibly a number component 

- Usage:
  ```tsx
  <RecipientsDisplay {recipients} />
  ```
-->

<div
  class="recipents"
  style={`width: ${divWidth}; overflow: hidden;text-overflow:ellipsis`}>
  <span>{recipients}</span>
</div>
