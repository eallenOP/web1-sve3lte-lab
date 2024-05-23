<script>
  import Header from "../components/Header.svelte";
  import Sidebar from "../components/Sidebar.svelte";
  import Footer from "../components/Footer.svelte";
 
</script>

<div class="container">
  <header><Header /></header>
  
 
    <slot />
  
  <footer><Footer /></footer>
</div>

<style>
    
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
  
</style>
