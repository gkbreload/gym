<script>
  import { openModal } from "../store";
</script>

<header class="flex flex-col relative z-20">
  <div
    class="max-w-[1400px] mx-auto w-full flex items-center justify-between p-4 py-6"
  >
    <a href="/">
      <h1 class="font-semibold">
        Swoley <span class="text-indigo-400">Moley</span>
      </h1>
    </a>
    <!-- svelte-ignore a11y_consider_explicit_label -->
    <button
      on:click={() => ($openModal = true)}
      class="md:hidden grid place-items-center"
    >
      <i class="fa-solid fa-bars"></i>
    </button>
    <nav class="hidden md:flex items-center gap-4 lg:gap-6">
      <a
        href="#product"
        class="duaration-200 hover:text-indigo-400 cursor-pointer">Product</a
      >
      <a
        href="#reviews"
        class="duaration-200 hover:text-indigo-400 cursor-pointer">Review</a
      >
      <a href="#faqs" class="duaration-200 hover:text-indigo-400 cursor-pointer"
        >FAQs</a
      >
      <button class="specialBtn">
        <p>Start free today</p>
      </button>
    </nav>
  </div>
</header>
