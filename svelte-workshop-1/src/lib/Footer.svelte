<script>
    const currentYear = new Date().getFullYear();
    const socialLinks = [
      { name: "GitHub", href: "https://github.com/ronitjena09", icon: "fab fa-github" },
      { name: "LinkedIn", href: "https://linkedin.com/in/ronitjena", icon: "fab fa-linkedin" },
      { name: "CodeForces", href: "https://codeforces.com/profile/ronitjena09", icon: "fab fa-codeforces" },
    ];
  </script>
  
  <footer class="bg-gray-800 text-white py-8">
    <div class="container mx-auto text-center">
      <div class="mb-6">
        <a href="/" class="text-3xl font-bold tracking-wider hover:text-gray-400">Ronit Jena</a>
      </div>
      <div class="mb-6">
        <ul class="flex justify-center space-x-6">
          {#each socialLinks as link}
            <li>
              <a href={link.href} class="text-xl hover:text-gray-400" target="_blank" rel="noopener noreferrer">
                <i class={link.icon}></i> <span class="sr-only">{link.name}</span>
              </a>
            </li>
          {/each}
        </ul>
      </div>
      <div class="mb-6">
        <p class="text-gray-400">&copy; {currentYear} Ronit Jena. All rights reserved.</p>
      </div>
      <div>
        <ul class="flex justify-center space-x-6 text-gray-400 text-sm">
          <li><a href="/privacy" class="hover:text-gray-200">Privacy Policy</a></li>
          <li><a href="/terms" class="hover:text-gray-200">Terms of Service</a></li>
          <li><a href="/contact" class="hover:text-gray-200">Contact Me</a></li>
        </ul>
      </div>
    </div>
  </footer>
  
  <style>
    @import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css');
  </style>
  