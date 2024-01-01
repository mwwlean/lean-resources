<script>
  import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
  import { DarkMode } from 'flowbite-svelte';

  let btnClass = 'text-gray-500 dark:text-gray-400 hover:bg-gray-100 dark:hover:bg-gray-700 rounded-lg text-xl p-2 md:p-0';
</script>

<Navbar class="bg-slate-100 dark:bg-gray-800 p-4 dark:border-slate-600 border-b border-slate-400">
  <NavBrand href="/">
    <span class="self-center whitespace-nowrap text-2xl font-bold text-orange-400 ">DDtools</span>
  </NavBrand>
  <NavHamburger />
    <NavUl>
      <NavLi href="/about" class="lg:text-base font-normal">About</NavLi>
      <NavLi href="/appdev" class="lg:text-base font-normal">Design Tools</NavLi>
      <NavLi href="/pricing" class="lg:text-base font-normal">Web Development Tools</NavLi>
      <NavLi href="/contact" class="lg:text-base font-normal">Mobile Development Tools</NavLi>
    <DarkMode {btnClass}/>
  </NavUl>
</Navbar>
