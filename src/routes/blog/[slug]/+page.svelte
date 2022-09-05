<script>
	export /**
	 * @type {{ title: any; date: any; Content: any; categories: any; }}
	 */
	let data;
	const { title, date, Content , categories } = data;
</script>

<svelte:head>
    <title>My blog - {title}</title>
    <meta property="og:title" content={title} />
</svelte:head>

<article>
	<h1>{data.title}</h1>
	<p>Published : {data.date}</p>
	{#if data.categories.length}
		<aside>
			<h2>Posted in:</h2>
			<ul>
				{#each data.categories as category}
					<li>
						<a href="/blog/category/{category}">
							{category}
						</a>
					</li>
				{/each}
			</ul>
		</aside>
	{/if}
	<svelte:component this={data.Content} />
</article>
