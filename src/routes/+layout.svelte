<script>
    import "../app.css";
    import Navbar from "$lib/components/navbar.svelte";
</script>
  

<div class="dark: dark:bg-[#191919] h-full pt-4 dark:text-[#F3F3F3] transition-colors ease-in-out">
    <Navbar />
    <slot />
</div>
