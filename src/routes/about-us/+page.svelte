<script>
  import Header from "../../components/Header.svelte";
  import SearchHeader from "../../components/SearchHeader.svelte";
  import Footer from "../../components/Footer.svelte";

  const member = [
    {
      name: "Yusril Izza Aulia",
      nim: 220401010039,
    },
    {
      name: "Rifky Al Fazar",
      nim: 220401010284,
    },
    {
      name: "Delia Rifatul Jannah",
      nim: 220401010077,
    },
  ];
</script>

<svelte:head>
  <title>AboutUs | BacaTech</title>
  <meta
    name="description"
    content="BacaTech is an online learning platform that offers various courses on programming, web development, and more."
  />
</svelte:head>
<Header />
<div class="flex p-5 h-screen flex-col items-center">
  <h2 class="text-2xl font-bold mt-4">About Us</h2>
  <h3 class="text-2xl font-bold">Kelompok 8 - IT 202</h3>
  <div class="overflow-x-auto mt-7">
    <table class="table">
      <!-- head -->
      <thead>
        <tr>
          <th />
          <th>Nim</th>
          <th>Name</th>
        </tr>
      </thead>
      <tbody>
        {#each member as m, i}
          <tr>
            <td>{i + 1}</td>
            <td>{m.nim}</td>
            <td>{m.name}</td>
          </tr>
        {/each}
      </tbody>
    </table>
  </div>

  <!-- embeded youtube video -->
  <div class="mt-10">
    <iframe
      width="560"
      height="315"
      src="https://www.youtube.com/embed/2Vv-BfVoq4g"
      title="YouTube video player"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    />
  </div>
</div>
<Footer />
