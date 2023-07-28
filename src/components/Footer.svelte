<script>
  import FaTwitter from "svelte-icons/fa/FaTwitter.svelte";
  import FaFacebookF from "svelte-icons/fa/FaFacebookF.svelte";
  import FaInstagram from "svelte-icons/fa/FaInstagram.svelte";
</script>

<footer>
  <div
    class="border px-4 md:px-10 py-4 flex items-center justify-between flex-wrap"
  />

  <div
    class="border px-4 md:px-10 py-1 flex items-center justify-between flex-wrap"
  >
    <div class="flex justify-start">
      <p class="text-gray-400 pr-7 py-2 rounded-md text-sm font-medium">
        &copy; 2023 - Baca Tech | All right reserved
      </p>
    </div>

    <div class="flex items-center">
      <div class="cursor-pointer mx-5 w-[20px] h-[20px]"><FaTwitter /></div>
      <div class="cursor-pointer mx-5 w-[20px] h-[20px]"><FaFacebookF /></div>
      <div class="cursor-pointer mx-5 w-[20px] h-[20px]"><FaInstagram /></div>
    </div>
  </div>
</footer>
