<script>
  export let item;
</script>

<li>
  <a
    href={item.link}
    class="flex items-center space-x-2 hover:bg-gray-200 rounded-l-lg py-2 px-2 cursor-pointer text-[.9375rem] text-[#050505]"
  >
    <slot name="icon" />

    <p class="text-md">{item.text}</p>
  </a>
</li>
