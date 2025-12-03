<script>
  const { label = 'Button', ...props } = $props();
</script>

<button
  {...props}
  class="cursor-pointer rounded-md bg-blue-300 px-2 text-blue-950 hover:bg-blue-400 hover:shadow-md"
  >{label}</button
>
