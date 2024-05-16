<script>
    export let navItems;
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
