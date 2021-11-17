<script>
  import PostBody from "./PostBody.svelte";
  import PostFooter from "./PostFooter.svelte";
  import PostHeader from "./PostHeader.svelte";
  import PostMedia from "./PostMedia.svelte";
</script>

<article class="rounded-lg shadow bg-white">
  <PostHeader />

  <PostBody />
  <PostMedia />

  <PostFooter />
</article>
