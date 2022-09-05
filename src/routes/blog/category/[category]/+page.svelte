<!-- src/routes/blog/+page.svelte -->
<script>
    // @ts-nocheck
        export let data;
    
</script>

<svelte:head>
    <title>Categories - {data.category}</title>
    <meta property="og:title" content={data.category} />
</svelte:head>


    <h1>Category {data.category}</h1>
    
    <ul>
        {#each data.posts as post}
            <li>
                <h2>
                    <a href={post.path}>
                        {post.meta.title}
                    </a>
                </h2>
                Published {post.meta.date}
            </li>
        {/each}
    </ul>
    