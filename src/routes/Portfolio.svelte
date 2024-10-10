<script>
  import { Link } from 'svelte-routing';
  
  let projects = [
    { name: 'Project 1', description: 'I made a pixelated moving mario through adobe.', image: '/images/Screenshot 2024-10-10 234830.jpg' },
    { name: 'Project 2', description: 'First time i made navigation bars.', image: '/images/Screenshot 2024-10-11 004931.jpg' },
    { name: 'Project 3', description: 'This is our first home page, we created a shoe website.', image: 'images/Screenshot 2024-10-11 005441.jpg' },
    { name: 'Project 4', description: 'This is the shoes that are inside of the shoe website we made.', image: 'images/Screenshot 2024-10-11 005511.jpg' },
  ];
</script>

<main class="p-8 bg-gray-300 min-h-screen">
  <h1 class="text-4xl font-bold text-center mb-8">My Portfolio</h1>
  <ul class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
    {#each projects as project}
      <li class="bg-gray-400 rounded-lg shadow-md transition-transform transform hover:scale-105 p-4">
        <img src={project.image} alt={project.name} style="width: 128px; height: 128px; object-fit: cover;" class="rounded-t-lg">
        <h2 class="text-xl font-semibold mt-4">{project.name}</h2>
        <p class="mt-2 text-gray-300">{project.description}</p>
      </li>
    {/each}
  </ul>
</main>
