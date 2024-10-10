<script>
    let name = '';
    let email = '';
    let message = '';
  
    const handleSubmit = () => {
      console.log('Form submitted with:', { name, email, message });
      // Add logic to handle form submission
    };
  </script>
  
  <main class="p-8">
    <h1 class="text-4xl font-bold">Contact Me</h1>
    <form on:submit|preventDefault={handleSubmit} class="space-y-4">
      <input type="text" bind:value={name} placeholder="Name" class="border p-2 w-full rounded">
      <input type="email" bind:value={email} placeholder="Email" class="border p-2 w-full rounded">
      <textarea bind:value={message} placeholder="Message" class="border p-2 w-full rounded"></textarea>
      <button type="submit" class="bg-blue-500 text-white py-2 px-4 rounded">Send</button>
    </form>
  </main>
  