<script>
  export let imageBgPosition;
  export let text;
</script>

<button
  class="px-4 py-2 flex items-center  justify-center space-x-2 hover:bg-gray-100 rounded-lg"
>
  <div class="flex place-items-center">
    <i
      style=" background-image: url('https://static.xx.fbcdn.net/rsrc.php/v3/yC/r/jrzbj1_5Jys.png'); background-position: {imageBgPosition}"
      class="bg-no-repeat bg-auto w-6 h-6 inline-block"
    />
  </div>

  <span class="text-gray-600 font-medium hidden md:block">{text}</span>
</button>
