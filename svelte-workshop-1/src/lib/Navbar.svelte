<script>
  export let brand = "Ronit Jena";
  export let links = [
    { name: "Home", href: "/" },
    { name: "About Me", href: "/about" },
    { name: "Work", href: "/services" },
    { name: "Contact Me", href: "/contact" },
  ];
</script>

<nav class="bg-gradient-to-r from-purple-400 via-pink-500 to-red-500 text-white p-4 shadow-lg">
  <div class="container mx-auto flex justify-between items-center">
    <a href="/" class="text-3xl font-bold tracking-wider hover:text-gray-200">{brand}</a>
    <ul class="flex space-x-6">
      {#each links as link}
        <li>
          <a href={link.href} class="text-lg font-medium hover:text-gray-200 transition duration-300 ease-in-out">{link.name}</a>
        </li>
      {/each}
    </ul>
  </div>
</nav>
