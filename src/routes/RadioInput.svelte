<script>
export let name
export let label=""
export let options

</script>


<label for={name} class="block text-sm font-medium text-gray-700">{label}</label>
<div class="relative bg-white rounded-md -space-y-px">
  {#each options as option, i}
  <!-- Checked: "bg-indigo-50 border-indigo-200 z-10", Not Checked: "border-gray-200" -->
  <label for={name} class="rounded-tl-md rounded-tr-md relative border p-4 flex flex-col cursor-pointer md:pl-4 md:pr-6 md:grid md:grid-cols-3 focus:outline-none">
    <div class="flex items-center text-sm">
      <input type="radio" name={name} value={option} class="h-4 w-4 text-indigo-600 border-gray-300 focus:ring-indigo-500" aria-labelledby="pricing-plans-0-label" aria-describedby="pricing-plans-0-description-0 pricing-plans-0-description-1">
      <!-- Checked: "text-indigo-900", Not Checked: "text-gray-900" -->
      <span id="{name}-{i}" class="ml-3 font-medium">{option}</span>
    </div>
  </label>
  {/each}
</div>
