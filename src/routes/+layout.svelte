<script>
  import Header from "../components/Header.svelte";
  import Sidebar from "../components/Sidebar.svelte";
  import Footer from "../components/Footer.svelte";
  let navItems = [
    { text: "Home", href: "/" },
    { text: "About", href: "/about" },
    { text: "My Cards", href: "/cards" },
    { text: "Contact", href: "/contact" },
  ];
</script>

<div class="container">
  <header><Header /></header>
  <div class="left-side"><Sidebar {navItems} /></div>
  <main>
    <slot />
  </main>
  <footer><Footer /></footer>
</div>

<style>
    main {
    display: flex;
    flex-wrap: wrap;
    gap: 1em;
    padding: 1em;
  }
  .container {
    /* make this a holy grail layout */
    display: grid;
    grid-template: auto 1fr auto / auto 1fr;
  }
  header {
    padding: 2rem;
    grid-column: 1 / 3;
    background-color: bisque;
  }
  footer {
    padding: 1.4em;
    grid-column: 1 / 3;
    background-color: aquamarine;
  }
  .left-side {
    padding: 1em;
    grid-column: 1 / 2;
    background-color: aliceblue;
  }
</style>
