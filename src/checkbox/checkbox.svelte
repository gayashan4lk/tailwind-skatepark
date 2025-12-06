<script>
  const { label = 'A Very Important Checkbox', id = 'checkbox', ...props } = $props();
</script>

<div
  class="rounded-md bg-slate-200 p-2 pl-4 outline-2 outline-slate-300 focus-within:bg-sky-200 focus-within:outline-sky-300"
>
  <input
    {id}
    {...props}
    class="accent-sky-500 focus:rounded-md focus:ring-2 focus:ring-pink-500 focus:ring-offset-0 focus:outline-none"
    type="checkbox"
  />
  <label for={id} class="ml-1 text-center font-semibold text-slate-900">{label}</label>
</div>
