<script>
  const { title = 'Card Title', description = 'Card description' } = $props();
</script>

<div class="w-[300px] rounded-md bg-teal-400 p-4 pt-20">
  <h2 class="mb-1 font-serif text-3xl font-bold antialiased">{title}</h2>
  <p class="mt-1 text-xs font-light antialiased">{description}</p>
</div>
