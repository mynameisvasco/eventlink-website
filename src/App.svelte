<script>
  import { Router, Route } from "svelte-routing";
  import Footer from "./components/Footer/Footer.svelte";
  import Navbar from "./components/Navbar/Navbar.svelte";
  import DocumentationPage from "./pages/Documentation/DocumentationPage.svelte";
  import HomePage from "./pages/Home/HomePage.svelte";
  import ProductPage from "./pages/Product/ProductPage.svelte";
  import TeamPage from "./pages/Team/TeamPage.svelte";
  export let url = "";
</script>

<Router {url}>
  <Navbar />
  <Route path="/" component={HomePage} />
  <Route path="/team" component={TeamPage} />
  <Route path="/product" component={ProductPage} />
  <Route path="/docs" component={DocumentationPage} />
  <Footer />
</Router>
