<script>
  import Button from "$lib/components/ui/button/button.svelte";
</script>

<div class="flex justify-center">
  <h1 class="font-bold">Create a New Task</h1>
</div>

<form class="mx-20 rounded-2xl bg-amber-100 px-10 py-5">
  <div class="">
    <label for="title">Title:</label>
    <input type="text" id="title" class="bg-gray-100 rounded-2xl" />
  </div>

  <div>
    <label for="description">Description:</label>
    <input type="text" id="description" />
  </div>

  <div>
    <label for="category">Category:</label>
    <select name="category" id="category">
      <option value="Coding">Coding</option>
      <option value="University">University</option>
      <option value="Health">Health</option>
    </select>
  </div>

  <Button variant="outline" class="bg-black text-white">Create</Button>
  <Button variant="outline" class="bg-black text-white" href="/">Back</Button>
</form>
