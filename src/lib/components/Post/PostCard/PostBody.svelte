<section class="px-4 flex flex-col space-y-2">
  <p class="text-[.9375rem] text-[#050505]">
    Follow along to learn what pipeline operators and piping are, how they work,
    and how to use them, as well as how to create your own pipe function in
    JavaScript.
  </p>

  <div class="flex items-center space-x-2">
    {#each ["#DEV Community", "#Open Source", "#Developer"] as tag}
      <a href="/" class="text-blue-500 hover:underline text-sm">
        {tag}
      </a>
    {/each}
  </div>
</section>
