<script>
  import Login from "$lib/components/Login.svelte";
</script>

<div class="bg-gray-100 min-h-screen flex place-items-center px-2">
  <div class="max-w-4xl mx-auto">
    <div class="grid grid-cols-1 md:grid-cols-2 gap-10 items-center">
      <section class="max-w-md mx-auto">
        <h1 class="text-blue-500 text-4xl md:text-6xl font-bold">Sveltebook</h1>

        <h6 class="mt-4 text-xl md:text-2xl">
          Sveltebook helps you connect and share with the people in your life.
        </h6>
      </section>

      <section>
        <div class="max-w-md mx-auto">
          <Login>
            <div slot="bottom">
              <div class="py-4 text-center">
                <a href="/" class="text-blue-500 text-sm"
                  >Forgotten password ?</a
                >
              </div>
              <hr class="py-4" />
              <div class="flex justify-center">
                <button
                  class="font-bold text-white px-4 py-3 rounded-md  bg-[#42b72a]"
                  >Create New Account</button
                >
              </div>
            </div>
          </Login>
        </div>
      </section>
    </div>
  </div>
</div>
