<script>
  export let extraClasses;
</script>

<div class={`bg-gray-100 h-screen fixed top-15 w-1/4 hidden ${extraClasses}`}>
  <slot />
</div>

