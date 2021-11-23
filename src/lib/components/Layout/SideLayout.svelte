<script>
  export let extraClasses;
</script>

<div class={`bg-gray-100 h-screen fixed top-14 w-1/4 hidden py-4 ${extraClasses}`}>
  <slot />
</div>

