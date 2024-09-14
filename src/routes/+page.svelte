<script>
  import Github from "$lib/assets/github.svelte";
  import Link from "$lib/assets/link.svelte";
  import Mail from "$lib/assets/mail.svelte";
</script>

<div class="flex flex-col justify-center items-center h-[calc(100vh-80px)]">

  <h1 class="text-7xl font-semibold">
    Cloudy
  </h1>

  <h2 class="font-semibold text-3xl text-center">
    Full Stack Dev
  </h2>

  <div class="flex mt-4">
    <a href="https://github.com/cloudyio">
      <Github />
    </a>
    <a href="#">
      <Mail />
    </a>
    <a href="#">
      <Link />
    </a>
  </div>

</div>

