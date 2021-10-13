<script>
export let name
export let label
export let placeholder=""
</script>

<label for={name} class="block text-sm font-medium text-gray-700">{label}</label>
<input type="text" name={name} id={name} placeholder={placeholder} class="placeholder-gray-300 mt-1 block w-full border border-gray-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm">
