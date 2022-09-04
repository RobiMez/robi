<!-- Header.svelte -->
<header>
    <a href="/">Home</a>
  
    <nav>
      <ul>
        <li>
          <a href="/blog">Blog</a>
        </li>
        <li>
          <a href="/about">About</a>
        </li>
        <li>
          <a href="/contact">Contact</a>
        </li>
      </ul>
    </nav>
  </header>


<style>

  header {
    padding: 1rem 2.5rem;
    color: #A7BC8A;
    background: #1F1E1E;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }
  
  ul {
    margin: 0;
    list-style-type: none;
    display: flex;
    gap: 1rem;
  }
  
  a {
    text-decoration: none;
    font-weight: 900;
    color: inherit;
  }
  a:hover {
    color: #CDDABF;
  }
</style>