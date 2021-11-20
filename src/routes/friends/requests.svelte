<script>
  import ViewSentRequests from "$lib/components/Friend/Sidebar/ViewSentRequests.svelte";

  import SideLayout from "$lib/components/Layout/SideLayout.svelte";
</script>

<SideLayout extraClasses="lg:block left-0 bg-white shadow px-4">
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

    <h4 class="text-2xl font-medium">Friend requests</h4>
  </div>
  <hr />

  <div class="pt-4 flex items-center space-x-4">
    <h6 class="text-md font-medium">Friend requests</h6>
  </div>

  <ViewSentRequests />

  <div>
    <p class="text-sm text-gray-500">No new requests</p>
  </div>
</SideLayout>

<div class="w-3/4">
  <div
    class="absolute grid place-items-center place-content-center"
  >
    <div class="flex flex-col items-center">
        <img
      src="https://www.facebook.com/images/comet/empty_states_icons/people/null_states_people_gray_wash.svg"
      alt="No Requests"
      class="w-32"
    />

    <p class="text-gray-500 font-medium text-lg">
      When you have friend requests or suggestions, you'll see them here.
    </p>
    </div>
  </div>
</div>
