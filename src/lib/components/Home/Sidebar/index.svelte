<script>
  import { text } from "svelte/internal";

  import ListItem from "./ListItem.svelte";

  const items = [
    {
      text: "Harsh Mangalam",
      src: "https://scontent.fpat3-1.fna.fbcdn.net/v/t1.30497-1/cp0/p40x40/143086968_2856368904622192_1959732218791162458_n.png?_nc_cat=1&ccb=1-5&_nc_sid=dbb9e7&_nc_ohc=OQSfMhmY6y0AX8QE5-3&_nc_ht=scontent.fpat3-1.fna&oh=85000593e0be81f5133dee98e80d12b7&oe=61BBFEA3",
      link: "/me",
    },
    {
      text: "Find Friends",
      src: "https://static.xx.fbcdn.net/rsrc.php/v3/y8/r/S0U5ECzYUSu.png",
      link: "/friends",
    },

    {
      text: "Groups",
      src: "https://static.xx.fbcdn.net/rsrc.php/v3/y5/r/PrjLkDYpYbH.png",
      link: "/groups",
    },
    {
      text: "Watch",
      src: "https://static.xx.fbcdn.net/rsrc.php/v3/y5/r/duk32h44Y31.png",
      link: "/marketplace",
    },
    {
      text: "Marketplace",
      src: "https://static.xx.fbcdn.net/rsrc.php/v3/yU/r/D2y-jJ2C_hO.png",
      link: "/watch",
    },
    {
      text: "Memories",
      src: "https://static.xx.fbcdn.net/rsrc.php/v3/y8/r/he-BkogidIc.png",
      link: "/memories",
    },
    {
      text: "Saved",
      src: "https://static.xx.fbcdn.net/rsrc.php/v3/yD/r/lVijPkTeN-r.png",
      link: "/saved",
    },
    {
      text: "Pages",
      src: "https://static.xx.fbcdn.net/rsrc.php/v3/yH/r/kyCAf2jbZvF.png",
      link: "/pages",
    },
    {
      text: "Events",
      src: "https://static.xx.fbcdn.net/rsrc.php/v3/yu/r/eXC82ZeepQ7.png",
      link: "/events",
    },

    {
      text: "Jobs",
      src: "https://static.xx.fbcdn.net/rsrc.php/v3/yY/r/XxEsb0x8INQ.png",
      link: "/jobs",
    },
  ];
</script>

<ul class="pl-2">
  {#each items as item (item.text)}
    <ListItem {item}>
      <img
        src={item.src}
        alt={item.text}
        class="rounded-full w-9 h-9"
        slot="icon"
      />
    </ListItem>
  {/each}

  <li class="pl-2 mt-6">
      <p class="text-sm text-gray-600">
        Sveltebook &copy; {new Date().getFullYear()}
      </p>
  </li>
</ul>
