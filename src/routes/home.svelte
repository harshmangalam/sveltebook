<script>
  import CreatePost from "$lib/components/Post/CreatePost.svelte";
import CreateRoom from "$lib/components/Room/CreateRoom.svelte";
  import CreateStory from "$lib/components/Story/CreateStory.svelte";
</script>

<div class="min-h-screen bg-gray-100 pt-4">
  <div class="max-w-xl mx-auto">
    <div>
      <CreateStory />
    </div>

    <div class="mt-4">
      <CreatePost />
    </div>

    <div class="mt-4">
      <CreateRoom />
    </div>
  </div>
</div>
