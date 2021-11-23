<script>
  import FriendCard from "$lib/components/Friend/Suggestions/FriendCard.svelte";
import SideLayout from "$lib/components/Layout/SideLayout.svelte";
</script>

<SideLayout extraClasses="lg:block left-0 bg-white shadow pl-4 overflow-y-scroll">
  <div class="pt-4 flex items-center space-x-4">
    <a href="/friends" class="p-2 hover:bg-gray-100 rounded-full">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="h-5 w-5"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M10 19l-7-7m0 0l7-7m-7 7h18"
        />
      </svg>
    </a>

    <h4 class="text-2xl font-medium">Suggestions</h4>
  </div>

  <div class="my-2">
    <h6 class="font-medium">People you may know</h6>

    <div class="my-2 grid grid-cols-1 mb-12">
        {#each [1,2,3,4,5,6,7,8,9] as friend}
          <FriendCard />
        {/each}
    </div>
  </div>
</SideLayout>

<div class="w-3/4">
  <div
    class="absolute top-1/2 left-1/2 transform -translate-y-1/2 -translate-x-1/4"
  >
    <div class="flex flex-col items-center space-y-4">
      <img
        src="https://www.facebook.com/images/comet/empty_states_icons/people/null_states_people_gray_wash.svg"
        alt="No Requests"
        class="w-32"
      />

      <p class="text-gray-500 font-bold text-xl">
        Select people's names to preview their profile.
      </p>
    </div>
  </div>
</div>
