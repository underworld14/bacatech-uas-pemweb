<script>
  import ArticleSidebar from "../../../components/creator/ArticleSidebar.svelte";
</script>

<svelte:head>
  <title>Creator | BacaTech</title>
  <meta
    name="description"
    content="Discover and explore the BacaTech Creator program, where you can build and share your own coding projects with the community."
  />
</svelte:head>

<div>
  <ArticleSidebar />
  <div class="ml-[300px]">
    <slot />
  </div>
</div>
