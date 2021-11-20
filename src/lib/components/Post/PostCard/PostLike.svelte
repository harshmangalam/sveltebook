<script>
  let dialog = false;

  function showDialog() {
    console.log("hi");
    dialog = true;
  }

  function hideDialog() {
    console.log("hi");
    dialog = false;
  }
</script>

<button
  class="px-4 py-2 flex items-center  justify-center space-x-2 hover:bg-gray-100 rounded"
>
  <div class="flex place-items-center">
    <i
      style=" background-image: url('https://static.xx.fbcdn.net/rsrc.php/v3/ys/r/gWdQco0HMJM.png'); background-position: 0px -222px"
      class="bg-no-repeat bg-auto w-5 h-5 inline-block"
    />
  </div>

  <span class="text-gray-600 font-medium hidden md:block">Like</span>
</button>

{#if dialog}
  <div
    class="bg-white rounded-full px-1 py-1 flex space-x-2 absolute -top-14 shadow border"
  >
    <button
      class="rounded-full hover:scale-125 hover:-translate-y-1 transition duration-500"
    >
      <img class="w-10 h-10" src="/images/like.png" alt="Like" />
    </button>
    <button
      class="rounded-full hover:scale-125 hover:-translate-y-1 transition duration-500"
    >
      <img class="w-10 h-10" src="/images/love.png" alt="Love" />
    </button>
    <button
      class="rounded-full hover:scale-125 hover:-translate-y-1 transition duration-500"
    >
      <img class="w-10 h-10" src="/images/care.png" alt="Care" />
    </button>
    <button
      class="rounded-full hover:scale-125 hover:-translate-y-1 transition duration-500"
    >
      <img class="w-10 h-10" src="/images/haha.png" alt="Haha" />
    </button>
    <button
      class="rounded-full hover:scale-125 hover:-translate-y-1 transition duration-500"
    >
      <img class="w-10 h-10" src="/images/wow.png" alt="Wow" />
    </button>
    <button
      class="rounded-full hover:scale-125 hover:-translate-y-1 transition duration-500"
    >
      <img class="w-10 h-10" src="/images/sad.png" alt="Sad" />
    </button>
    <button
      class="rounded-full hover:scale-125 hover:-translate-y-1 transition duration-500"
    >
      <img class="w-10 h-10" src="/images/angry.png" alt="Angry" />
    </button>
  </div>
{/if}
