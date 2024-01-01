<script>
  import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
  import { DarkMode } from 'flowbite-svelte';

  let btnClass = 'text-gray-500 dark:text-gray-400 hover:bg-gray-100 dark:hover:bg-gray-700 rounded-lg text-xl p-2 md:p-0';
</script>

<Navbar class="bg-slate-200">
  <NavBrand href="/">
    <span class="self-center whitespace-nowrap text-xl font-bold dark:text-white ">Devtools</span>
  </NavBrand>
  <NavHamburger />
  <NavUl>
    <NavLi href="/about">About</NavLi>
    <NavLi href="/appdev">App</NavLi>
    <NavLi href="/pricing">Pricing</NavLi>
    <NavLi href="/contact">Contact</NavLi>
    <DarkMode {btnClass} />
  </NavUl>
</Navbar>

<style>

</style>