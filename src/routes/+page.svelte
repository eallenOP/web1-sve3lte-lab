<script>
    import Header from '../components/Header.svelte';
    import Card from '../components/Card.svelte';
    import Sidebar from '../components/Sidebar.svelte'
    import Footer from '../components/Footer.svelte';
</script>

<Header />
<Sidebar />
<main>
    <Card />
    <Card />
</main>
<Footer />

<style>
    main {
        display: flex;
    }
</style>