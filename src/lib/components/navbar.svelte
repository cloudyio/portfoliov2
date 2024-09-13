<script>
    import sun from "$lib/assets/sun.svg";
</script>

<nav class="h-14 mx-5 mt-3 rounded-full bg-[#D9D9D9] relative text-xl font-inter md:text-2xl">
    <a href="https://example.com" class="absolute transform top-1/2 -translate-y-1/2 ml-5">
        <img src={sun} class="h-8 w-10" alt="sun" />
    </a>

    <div class="absolute right-5 top-1/2 transform -translate-y-1/2 text-sm md:text-base lg:text-lg">
        <a href="#" class="mr-4 font-semibold">My Projects</a>
        <a href="#" class="mr-4 font-semibold">About Me</a>
        <a href="#" class="font-semibold mr-4">Contact</a>
    </div>
</nav>
