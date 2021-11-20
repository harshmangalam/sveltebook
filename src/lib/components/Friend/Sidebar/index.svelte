<script>
  let items = [
    {
      name: "Friend requests",
      bgPosition: "0px -264px",
      link: "/friends/requests",
      showChev: true,
    },
    {
      name: "Suggestions",
      bgPosition: "0px -222px",
      link: "/friends/suggestions",
      showChev: true,
    },
    {
      name: "All Friends",
      bgPosition: "0px -243px",
      link: "/friends/list",
      showChev: true,
    },
    {
      name: "Birthdays",
      bgPosition: "0px -306px",
      link: "/friends/birthdays",
      showChev: false,
    },
    {
      name: "Custom lists",
      bgPosition: "0px -243px",
      link: "/friends/friendlist",
      showChev: true,
    },
  ];
</script>

<ul>
  <li>
    <a
      href="/friends"
      class="flex items-center justify-between bg-gray-100 py-2 px-2 rounded-lg"
    >
      <div class="flex items-center space-x-4">
        <div class="flex place-items-center p-2 bg-blue-500 rounded-full">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-5 w-5 text-white"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              d="M9 6a3 3 0 11-6 0 3 3 0 016 0zM17 6a3 3 0 11-6 0 3 3 0 016 0zM12.93 17c.046-.327.07-.66.07-1a6.97 6.97 0 00-1.5-4.33A5 5 0 0119 16v1h-6.07zM6 11a5 5 0 015 5v1H1v-1a5 5 0 015-5z"
            />
          </svg>
        </div>
        <p>Home</p>
      </div>
    </a>
  </li>

  {#each items as item (item.name)}
    <li>
      <a
        href={item.link}
        class="flex items-center justify-between hover:bg-gray-100 px-2 py-2 rounded-lg"
      >
        <div class="flex items-center space-x-4">
          <div class="flex place-items-center p-2 bg-gray-200 rounded-full">
            <i
              style="background-image: url('https://static.xx.fbcdn.net/rsrc.php/v3/yf/r/jg33dXF5j3w.png');background-position: {item.bgPosition}"
              class="bg-no-repeat bg-auto w-5 h-5 inline-block"
            />
          </div>
          <p>{item.name}</p>
        </div>

        {#if item.showChev}
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-6 w-6"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M9 5l7 7-7 7"
            />
          </svg>
        {/if}
      </a>
    </li>
  {/each}
</ul>
