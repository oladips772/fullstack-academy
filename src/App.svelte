<script>
import Footer from "./components/Footer.svelte";
import Header from "./components/Header.svelte";
import Info from "./components/Info.svelte";
import Stack from "./components/Stack.svelte";
import Tech from "./components/Tech.svelte";
import {
    Router,
    Link,
    Route
} from "svelte-routing";
import Login from "./components/Login.svelte";
import CoursePage from "./components/CoursePage.svelte";
</script>

<Router>
    <main>
        <Route path="/Login">
            <Login />
        </Route>
        <Route path="/Courses">
            <Header />
            <CoursePage />
            <Footer />
        </Route>
        <Route exact path="/">
            <Header />
            <div class="app-body">
                <Info />
                <Stack />
                <Tech />
            </div>
            <Footer />
        </Route>
    </main>
</Router>

<style>
.app-body {
    height: calc(100% - 60px);
    margin: 0px 70px 0px 70px;
}
</style>
