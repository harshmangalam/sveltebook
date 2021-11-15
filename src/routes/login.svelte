<script>
  import Login from "$lib/components/Login.svelte";
</script>

<div class="bg-gray-100 min-h-screen flex flex-col  justify-between">
  <section class="max-w-sm mx-auto pt-12">
    <h1 class="text-blue-500 text-4xl font-bold text-center">Sveltebook</h1>
    <div class="mt-6">
      <Login>
        <div slot="top" class="mb-6">
          <h6 class="text-center text-xl">Log in to sveltebook</h6>
        </div>

        <div class="mt-6 grid grid-cols-2 gap-2" slot="bottom">
          <a href="/" class="text-sm text-blue-500">Forgotten account ?</a>
          <a href="/" class="text-sm text-blue-500">Sign up for Sveltebook ?</a>
        </div>
      </Login>
    </div>
  </section>

  <section class="py-6 bg-white">
    <p class="text-center text-gray-400">
      Sveltebook &copy; {new Date().getFullYear()}
    </p>
  </section>
</div>
