<script>
  import { Navbar, NavBrand, NavHamburger, NavUl, NavLi, MegaMenu } from 'flowbite-svelte';
  import { IconOutline, ChevronDownOutline } from 'flowbite-svelte-icons';
  import { DarkMode } from 'flowbite-svelte';
  let name = "</>";
  let btnClass = 'text-gray-500 dark:text-gray-400 hover:bg-gray-100 dark:hover:bg-gray-700 rounded-lg text-xl p-2 md:p-0';
</script>

<Navbar let:hidden let:toggle class="bg-neutral-100 dark:bg-gray-800 p-2 dark:border-gray-700 border-b border-slate-300 font-mono">
  <NavBrand href="/">
    <span class="self-center whitespace-nowrap text-2xl font-extrabold text-orange-400">{name}</span>
  </NavBrand>
  <NavHamburger />
  <NavUl>
    <NavLi href="/all-pages" class="sm:hidden">All</NavLi>
    <NavLi href="/design-pages" class="sm:hidden">Design</NavLi>
    <NavLi href="/frontend-pages" class="sm:hidden">Frontend Tools</NavLi>
    <NavLi href="/backend-pages" class="sm:hidden">Backend Tools</NavLi>
    <NavLi href="/courses-pages" class="sm:hidden">Coding Courses</NavLi>
    <NavLi href="/documentations-pages" class="sm:hidden">Documentations</NavLi>
    <NavLi href="/icons-pages" class="sm:hidden">Icons</NavLi>
    <NavLi href="/colors-pages" class="sm:hidden">Colors</NavLi>
    <NavLi href="/typography-pages" class="sm:hidden">Typography</NavLi>

    <DarkMode {btnClass}/>  
  </NavUl>
   
</Navbar>