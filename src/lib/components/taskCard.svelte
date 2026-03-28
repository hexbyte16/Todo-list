<script>
  let { title, description, status, color, completed, category } = $props();
  import Button from "$lib/components/ui/button/button.svelte";
</script>

<article
  class="rounded-2xl p-5 space-y-5 m-5"
  style="background-color: {color};"
>
  <div>
    <span class="bg-black text-white p-2 rounded-2xl">{category}</span>
  </div>
  <div>
    <h2 class="font-bold text-2xl">{title}</h2>
    <p>{description}</p>
  </div>
  <div>
    <Button
      variant="outline"
      onclick={() => {
        status = completed;
      }}>{status}</Button
    >
    <Button variant="outline" class="bg-red-500 text-white">Delete</Button>
  </div>
</article>
