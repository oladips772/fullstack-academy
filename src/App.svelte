<script>
  import Footer from "./components/Footer.svelte";
  import Header from "./components/Header.svelte";
  import Info from "./components/Info.svelte";
  import Stack from "./components/Stack.svelte";
  import Tech from "./components/Tech.svelte";
  import { Router, Link, Route } from "svelte-routing";
  import Login from "./components/Login.svelte";
</script>

<Router>
  <main>
    <Route exact path="/Login" component={Login}>
      <Login />
    </Route>
    <Route exact path="/">
      <Header />
      <div class="app-body">
        <Info />
        <Tech />
        <Stack />
      </div>
      <Footer />
    </Route>
  </main>
</Router>

<!-- GET a new immport -->
<style>
  .app-body {
    height: calc(100% - 60px);
    margin: 0px 70px 0px 70px;
  }
</style>
