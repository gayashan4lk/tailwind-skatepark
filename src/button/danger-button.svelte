<script>
  const { label = 'Button', ...props } = $props();
</script>

<button
  {...props}
  class="cursor-pointer rounded-md bg-rose-500 px-2 text-white hover:bg-rose-700 hover:shadow-md"
  >{label}</button
>
