<script>
    import { Link } from 'svelte-routing';
    let name = '';
    let email = '';
    let message = '';
  
    const handleSubmit = () => {
      console.log('Form submitted with:', { name, email, message });
      name = '';
      email = '';
      message = '';
    };
  </script>
  
  <main class="p-8 bg-gray-100 min-h-screen">
    <h1 class="text-4xl font-bold text-center mb-4">Contact Me</h1>
    <form on:submit|preventDefault={handleSubmit} class="max-w-md mx-auto bg-white p-6 rounded-lg shadow-lg space-y-4">
      <input type="text" bind:value={name} placeholder="Name" class="border border-gray-300 p-2 w-full rounded focus:outline-none focus:ring focus:ring-blue-500" required>
      <input type="email" bind:value={email} placeholder="Email" class="border border-gray-300 p-2 w-full rounded focus:outline-none focus:ring focus:ring-blue-500" required>
      <textarea bind:value={message} placeholder="Message" class="border border-gray-300 p-2 w-full rounded focus:outline-none focus:ring focus:ring-blue-500" required></textarea>
      <button type="submit" class="bg-blue-500 text-white py-2 px-4 rounded-lg hover:bg-blue-600 transition">Send</button>
    </form>
  </main>
  