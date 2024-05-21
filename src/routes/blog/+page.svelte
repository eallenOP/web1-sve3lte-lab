<script>
  let articles = [
    {
      slug: "cats",
      title: "Cats are the internet",
      body: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Repellat incidunt eum consectetur beatae labore facilis. Fugit amet inventore eaque quo reprehenderit maiores atque reiciendis vero voluptate! Reiciendis eligendi ut distinctio.",
    },
    {
      slug: "breakfast",
      title: "Breakfast are the internet",
      body: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Repellat incidunt eum consectetur beatae labore facilis. Fugit amet inventore eaque quo reprehenderit maiores atque reiciendis vero voluptate! Reiciendis eligendi ut distinctio.",
    },
  ];
</script>

<h1>My blog page</h1>

<ul>
  {#each articles as article}
    <li><a href="/blog/{article.slug}">{article.title}</a></li>
  {/each}
</ul>
