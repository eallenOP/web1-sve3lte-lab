<script>
    import Header from "../components/Header.svelte";
    import Card from "../components/Card.svelte";
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
    <Header />
    <Sidebar {navItems} />
    <main>
        <Card />
        <Card />
    </main>
    <Footer />
</div>

<style>
    main {
        display: flex;
        gap: 1em;
    }
    .container {
        /* make this a holy grail layout */
    }
</style>
