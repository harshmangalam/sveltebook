<script>
  import SideLayout from "$lib/components/Layout/SideLayout.svelte";
  import Sidebar from "$lib/components/Friend/Sidebar/index.svelte";

  const items = [
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

<SideLayout extraClasses="lg:block left-0 bg-white shadow px-2">
  <div class="flex items-center justify-between px-2 ">
    <h3 class="font-bold text-2xl">Friends</h3>
    <button class="bg-gray-100 p-2 rounded-full hover:bg-gray-200">
      <div class="flex place-items-center">
        <i
          style="background-image: url('https://static.xx.fbcdn.net/rsrc.php/v3/yP/r/auNLLvVwqJ4.png');background-position: 0px -305px;"
          class="bg-no-repeat bg-auto w-5 h-5 inline-block"
        />
      </div>
    </button>
  </div>
  <div class="mt-2">
    <Sidebar {items} />
  </div>
</SideLayout>

<div class="lg:w-3/4 ml-auto w-full">
  <slot />
</div>
