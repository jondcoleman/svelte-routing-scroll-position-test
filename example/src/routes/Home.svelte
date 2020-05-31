<script>
  import { Link } from "svelte-routing";
  const articles = [];
  for (let index = 0; 1 == 1; index++) {
    articles.push(`blog/${index}`);
    if (index > 100) break;
  }
</script>

<h1>Home</h1>
<p>Welcome to my website</p>
<ul>
  {#each articles as article}
    <li>
      <Link to={article}>{article}</Link>
    </li>
  {/each}
</ul>
