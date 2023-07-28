<script>
  import logo from "../lib/Logo.png";
  import Sidebar from "./Sidebar.svelte";

  const routes = [
    {
      href: "/articles",
      title: "Articles",
    },
    {
      href: "/forum",
      title: "Forum",
    },
  ];

  let isOpen = false;

  function toggleMenu() {
    isOpen = !isOpen;
  }
</script>

<Sidebar {toggleMenu} {isOpen} />
<header
  class="z-10 fixed shadow inset-x-0 top-0 flex items-center justify-between flex-wrap bg-primary py-3 px-5 md:px-10"
>
  <a href="/" class="hidden lg:block text-lg"> BacaTech </a>

  <div class="lg:hidden flex flex-col items-center justify-center">
    <button class="text-dark" on:click={toggleMenu}>
      <svg
        class="w-6 h-6"
        fill="none"
        stroke="currentColor"
        viewBox="0 0 24 24"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M4 6h16M4 12h16M4 18h16"
        />
      </svg>
    </button>
  </div>
  <div class="hidden lg:flex justify-center w-full md:w-auto">
    {#each routes as route}
      <a
        href={route.href}
        class="text-black hover:text-blue-600 px-4 md:px-7 py-2 rounded-md text-sm font-medium"
        >{route.title}</a
      >
    {/each}
  </div>
</header>
