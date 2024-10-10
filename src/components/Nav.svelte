<script>
    let links = [
      { name: 'Home', href: '/' },
      { name: 'Portfolio', href: '/portfolio' },
      { name: 'About', href: '/about' },
      { name: 'Contact', href: '/contact' }
    ];
  </script>
  
  <nav class="bg-blue-500 p-4 text-white">
    <ul class="flex space-x-4">
      {#each links as link}
        <li>
          <a href={link.href} class="hover:underline">{link.name}</a>
        </li>
      {/each}
    </ul>
  </nav>
  