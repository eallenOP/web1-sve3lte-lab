<script>
    let navItems = [
        { text: "Home", href: "/" },
        { text: "About", href: "/about" },
        { text: "My Cards", href: "/cards" },
        { text: "Contact", href: "/contact" },
        { text: "Cats", href: "/cats" },
    ];
</script>

<nav>
    <ul>
        {#each navItems as item}
            <li><a href={item.href}>{item.text}</a></li>
        {/each}
    </ul>
</nav>

<style>
    ul {
        padding-left: 0;
    }
    li {
        list-style: none;
    }
</style>
