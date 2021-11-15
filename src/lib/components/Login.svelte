<div class="shadow-md py-6 px-4 rounded-lg bg-white">
  
  <slot name="top" />
  
  <form class="grid grid-cols-1 gap-4">
    <div>
      <label for="username" />
      <input
        type="text"
        placeholder="Email address or phone number"
        class="text-lg focus:outline-none focus:placeholder-gray-400 placeholder-gray-500 w-full text-black border border-gray-300 rounded-md  px-4 py-3"
      />
    </div>
    <div>
      <label for="password" />
      <input
        type="password"
        placeholder="Password"
        class="text-lg focus:outline-none focus:placeholder-gray-400 placeholder-gray-500 w-full text-black border border-gray-300 rounded-md  px-4 py-3"
      />
    </div>
    <button
      class="bg-blue-500 text-white block w-full text-lg font-bold hover:bg-blue-600 rounded-md px-4 py-3"
    >
      Log In
    </button>
  </form>

  <slot name="bottom" />
</div>
