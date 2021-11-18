<script>
  import "../app.css";
  import Navbar from "$lib/components/Header/Navbar.svelte";
</script>

<div class="bg-gray-100 min-h-screen flex flex-col space-y-4">
  <Navbar />
  <main class="flex-grow px-2">
    <slot />
  </main>
</div>

