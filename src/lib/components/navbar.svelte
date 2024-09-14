<script>
    import sun from "$lib/assets/sun.svg";
    import moon from "$lib/assets/moon.svg";
  
    let isDarkMode = false;
  
    if (typeof window !== 'undefined') {
      isDarkMode = localStorage.getItem('theme') === 'dark';
  
      if (isDarkMode) {
        document.documentElement.classList.add('dark');
      } else {
        document.documentElement.classList.remove('dark');
      }
    }
  
    function toggleDarkMode() {
      isDarkMode = !isDarkMode;
  
      if (isDarkMode) {
        document.documentElement.classList.add('dark');
        localStorage.setItem('theme', 'dark');
      } else {
        document.documentElement.classList.remove('dark');
        localStorage.setItem('theme', 'light');
      }
    }
  </script>
  
  <nav class="h-16 mx-4 rounded-full bg-[#D9D9D9] dark:bg-[#292929] flex items-center justify-between px-6 text-xl font-inter transition-colors duration-500 ease-in-out">
    <button class="relative flex items-center" on:click={toggleDarkMode}>
      <img
        src={moon}
        class="h-9 w-9 transition-transform transform duration-500 ease-in-out 
          {isDarkMode ? 'scale-0 rotate-180 opacity-0' : 'scale-100 rotate-0 opacity-100'}"
        alt="moon"
      />
      <img
        src={sun}
        class="h-9 w-9 absolute transition-transform transform duration-500 ease-in-out 
          {isDarkMode ? 'scale-100 rotate-0 opacity-100' : 'scale-0 rotate-180 opacity-0'}"
        alt="sun"
      />
    </button>
  
    <div class="flex items-center space-x-6 md:text-lg text-xl">
      <a href="#" class="font-semibold">My Projects</a>
      <a href="#" class="font-semibold">About Me</a>
      <a href="#" class="font-semibold">Contact</a>
    </div>
  </nav>
  