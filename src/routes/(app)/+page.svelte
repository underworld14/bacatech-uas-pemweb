<script>
  import Footer from "../../components/Footer.svelte";
  import Header from "../../components/Header.svelte";
  import Features from "../../components/homepage/Features.svelte";
  import Hero from "../../components/homepage/Hero.svelte";
  import Info from "../../components/homepage/Info.svelte";
  import Subscribe from "../../components/homepage/Subscribe.svelte";
  import Testimony from "../../components/homepage/Testimony.svelte";
</script>

<svelte:head>
  <title>Homepage | BacaTech</title>
  <meta
    name="description"
    content="Progate is an online learning platform that offers various courses on programming, web development, and more."
  />
</svelte:head>
<div>
  <Header />
  <div class="overflow-hidden">
    <Hero />
    <Info />
    <Features />
    <Testimony />
    <Subscribe />
  </div>
  <Footer />
</div>
