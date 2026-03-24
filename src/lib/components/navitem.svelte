<script>
  const navItems = [
    { label: "Home", href: "/" },
    { label: "Settings", href: "settings" },
    { label: "Login", href: "sign-in" },
  ];
</script>

<nav class="flex items-center gap-4">
  {#each navItems as item}
    <a href={item.href}>{item.label}</a>
  {/each}
</nav>
