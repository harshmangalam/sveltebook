<script>
  import CreatePost from "$lib/components/Post/CreatePost.svelte";
  import PostCard from "$lib/components/Post/PostCard/index.svelte";
  import CreateRoom from "$lib/components/Room/CreateRoom.svelte";
  import CreateStory from "$lib/components/Story/CreateStory.svelte";
  import Sidebar from "$lib/components/Home/Sidebar/index.svelte";
  import SideLayout from "$lib/components/Layout/SideLayout.svelte";
  import UploadProfilePic from "$lib/components/Home/UploadProfilePic.svelte";
  import FriendListItem from "$lib/components/Friend/ListItem.svelte";
  import PeopleYouMayKnow from "$lib/components/Home/PeopleYouMayKnow.svelte";
</script>

<SideLayout extraClasses="lg:block left-0">
  <Sidebar />
</SideLayout>

<SideLayout extraClasses="lg:block right-0">
  <div class="flex flex-col space-y-4">
    <h2 class="text-lg font-medium text-gray-500">Group conversations</h2>
    <button
      class="flex items-center space-x-2 hover:bg-gray-200 py-2 px-2 rounded-lg"
    >
      <div class="bg-gray-300 p-2 rounded-full">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-5 w-5 text-black"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M12 4v16m8-8H4"
          />
        </svg>
      </div>
      <span class="text-sm font-weight-500">Create New Group</span>
    </button>
  </div>
</SideLayout>

<div class="flex justify-center">
  <div class="flex flex-col space-y-4 max-w-xl lg:max-w-lg xl:max-w-xl">
    <CreateStory />

    <CreatePost />

    <CreateRoom />

    <div class="mt-4 grid grid-cols-1 gap-4">
      {#each [1, 2, 3, 4, 5, 6] as post}
        <PostCard />
      {/each}
    </div>
    <h6 class="font-medium text-2xl">Welcome to Sveltebook, Harsh</h6>

    <UploadProfilePic />

    <div
      class="mt-4 grid grid-cols-1 gap-4 bg-white rounded-lg py-4 px-6 shadow"
    >
      <h3 class="font-medium text-xl">Add People You know</h3>
      <ul class=" divide-y">
        {#each [1, 2, 3, 4, 5, 6] as friend}
          <FriendListItem />
        {/each}
      </ul>
    </div>

    <div
      class="mt-4 grid grid-cols-1 gap-4 bg-white rounded-lg py-4 px-6 shadow"
    >
      <div class="flex items-center justify-between">
        <h3 class="font-bold text-gray-500 text-md">People You May know</h3>
        <button class="rounded-full p-2 hover:bg-gray-100">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-5 w-5 text-gray-500"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M5 12h.01M12 12h.01M19 12h.01M6 12a1 1 0 11-2 0 1 1 0 012 0zm7 0a1 1 0 11-2 0 1 1 0 012 0zm7 0a1 1 0 11-2 0 1 1 0 012 0z"
            />
          </svg>
        </button>
      </div>
      <ul class="grid grid-cols-3 gap-2">
        {#each [1, 2, 3] as friend}
          <PeopleYouMayKnow />
        {/each}
      </ul>
    </div>
  </div>
</div>
