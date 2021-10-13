<script>
export let name
export let label=""
export let options
export let placeholder=0
</script>



<label for={name} class="block text-sm font-medium text-gray-700">{label}</label>
<select id={name} name={name} class="mt-1 block w-full pl-3 pr-10 py-2 text-base border-gray-300 focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm rounded-md">
  {#each options as option, i}
    {#if placeholder==i}
      <option selected>{option}</option>
    {:else}
      <option>{option}</option>
    {/if}
  {/each}
</select>
