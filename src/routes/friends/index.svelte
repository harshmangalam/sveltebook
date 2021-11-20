<script>
  import FriendCard from "$lib/components/Friend/Sidebar/FriendCard.svelte";
</script>

<div class="pt-4 md:px-8">
  <div class="flex justify-between items-center mb-4">
    <h4 class="text-xl font-medium">
      People you may know
    </h4>
    <a href="/friends/suggestions" class="text-blue-500 py-2 px-2 hover:bg-gray-200 rounded">
    See all</a>
  </div>
  <div class="grid grid-cols-2 md:grid-cols-4 xl:grid-cols-5 gap-3">
    {#each [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20] as friend}
      <FriendCard />
    {/each}
  </div>
</div>
