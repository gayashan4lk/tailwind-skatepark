<script>
  const { label = 'Button', ...props } = $props();
</script>

<button
  {...props}
  class="cursor-pointer rounded-md bg-blue-500 px-2 text-white hover:bg-blue-600 hover:shadow-md"
>
  {label}
</button>
