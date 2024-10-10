<script>
  import { Link } from 'svelte-routing';
</script>

<nav class="bg-gray-600 p-4 shadow-lg ">
  <div class="container mx-auto">
    <ul class="flex space-x-6">
      <li>
        <Link to="/" class="text-gray-300 font-semibold transition duration-300">Home</Link>
      </li>
      <li>
        <Link to="/portfolio" class="text-gray-300 font-semibold transition duration-300">Portfolio</Link>
      </li>
      <li>
        <Link to="/about" class="text-gray-300 font-semibold  transition duration-300">About</Link>
      </li>
      <li>
        <Link to="/contact" class="text-gray-300 font-semibold transition duration-300">Contact</Link>
      </li>
    </ul>
  </div>
</nav>
