<script lang="ts">
  export let highlight: {
    icon: ConstructorOfATypedSvelteComponent;
    title: string;
    description: string;
  };
  export let Icon = highlight.icon;
</script>

<div class="mt-5 w-72">
  <div class="flex md:block space-x-2 md:space-x-0">
    <i
      class="bg-slate-100 border w-12 border-slate-200 p-2.5 text-xl flex justify-center items-center rounded-lg"
    >
      <svelte:component this={Icon} />
    </i>
    <div>
      <h1 class="text-lg my-2 font-semibold">{highlight.title}</h1>
    </div>
  </div>
  <p class="font-light text-slate-500 mt-2 md:mt-0">
    {highlight.description}
  </p>
</div>
