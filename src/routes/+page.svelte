<script>
  import TaskCard from "$lib/components/taskCard.svelte";
  import Button from "$lib/components/ui/button/button.svelte";
</script>

<h1 class="font-bold text-4xl m-10">Today Tasks</h1>
<Button variant="outline" class="bg-gray-100 text-black text-2xl" href="/new"
  >New Task</Button
>
<div class="md:flex">
  <TaskCard
    title="Study Math"
    description="today i must study math for 2 hours"
    completed="completed"
    status="incomplete"
    color="#ffda6e"
    category="university"
  />

  <TaskCard
    title="Make a video game"
    description="i should make a small video using unity"
    status="incomplete"
    color="#e5d0ff"
    completed="completed"
    category="Coding"
  />

  <TaskCard
    title="Do a morning run"
    description="Run for 30 minutes"
    status="incomplete"
    color="#BDE7FF"
    completed="completed"
    category="Health"
  />
</div>
