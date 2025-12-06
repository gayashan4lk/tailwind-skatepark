<script>
  const { id = 'input', label, description, error, ...props } = $props();
  const descriptionId = description ? `${id}-description` : undefined;
  const errorId = error ? `${id}-error` : undefined;
</script>

<div class="space-y-1.5">
  <label for={id} class="text-md block font-semibold text-slate-900">{label}</label>
  <input
    {id}
    aria-describedby={descriptionId}
    aria-invalid={!!error}
    aria-errormessage={errorId}
    {...props}
    class="block w-full rounded-md bg-slate-50 px-2 py-1 outline-2 outline-slate-200 focus:outline-2 focus:outline-blue-400"
  />
  {#if description}
    <p id={descriptionId}>{description}</p>
  {/if}
  {#if error}
    <p id={errorId}>{error}</p>
  {/if}
</div>
