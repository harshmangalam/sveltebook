<script>
  import FeatureButton from "./FeatureButton.svelte";
</script>

<div class="px-3 py-3 shadow bg-white rounded-lg">
  <div class="flex items-center space-x-2">
    <div class="flex-shrink-0">
      <img
        src="https://scontent.fpat3-3.fna.fbcdn.net/v/t1.30497-1/cp0/p50x50/143086968_2856368904622192_1959732218791162458_n.png?_nc_cat=1&amp;ccb=1-5&amp;_nc_sid=7206a8&amp;_nc_ohc=OQSfMhmY6y0AX8oaitX&amp;_nc_ht=scontent.fpat3-3.fna&amp;oh=710720f052b077740fa39c0834e2860d&amp;oe=61B79022"
        alt="profile"
        class="rounded-full w-10 h-10"
      />
    </div>
    <div
      class="w-full px-4 py-2 bg-gray-100 hover:bg-gray-200 rounded-full cursor-pointer"
    >
      <h3 class="md:text-md text-gray-500">What`s on your mind, Harsh ?</h3>
    </div>
  </div>
  <hr class="mt-3 mb-3" />
  <div class="grid grid-cols-3 gap-1">
    <FeatureButton text="Live video" imageBgPosition="0px 0px" />
    <FeatureButton text="Photo/Video" imageBgPosition="0px -225px" />
    <FeatureButton text="Feeling/Activity" imageBgPosition="0px -25px" />
  </div>
</div>
