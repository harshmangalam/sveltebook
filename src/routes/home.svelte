<script>
  import CreatePost from "$lib/components/Post/CreatePost.svelte";
  import PostCard from "$lib/components/Post/PostCard/index.svelte";
  import CreateRoom from "$lib/components/Room/CreateRoom.svelte";
  import CreateStory from "$lib/components/Story/CreateStory.svelte";
  import Sidebar from "$lib/components/Sidebar/index.svelte";
  import SideLayout from "$lib/components/Layout/SideLayout.svelte";
</script>

<SideLayout extraClasses="lg:block left-0 overflow-y-scroll">
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
  </div>
</div>


