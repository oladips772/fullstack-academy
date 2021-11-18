<script>
  import Footer from "./components/Footer.svelte";
  import Header from "./components/Header.svelte";
  import Info from "./components/Info.svelte";
  import Stack from "./components/Stack.svelte";
  import Tech from "./components/Tech.svelte";
</script>

<main>
  <Header />
  <div class="app-body">
    <Info />
    <Tech />
    <Stack />
  </div>
  <Footer />
</main>
<!-- GET a new immport -->
<style>
  .app-body {
    height: calc(100% - 60px);
    margin: 0px 70px 0px 70px;
  }
</style>
