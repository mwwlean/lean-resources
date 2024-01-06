<script>
  import { Navbar, NavBrand, NavHamburger, NavUl, NavLi, MegaMenu } from 'flowbite-svelte';
  import { IconOutline, ChevronDownOutline } from 'flowbite-svelte-icons';
  import { DarkMode } from 'flowbite-svelte';
  let menu = [
    { name: 'Design', href: '/design-pages', icon: 'user-circle-outline' },
    { name: 'Frontend', href: '/frontend-pages', icon: 'user-circle-outline' },
    { name: 'Backend', href: '/backend-pages', icon: 'user-circle-outline' },
    { name: 'Courses', href: '/courses-pages', icon: 'user-circle-outline' },
    { name: 'Icons', href: '/icons-pages', icon: 'user-circle-outline' },
    { name: 'Documentations', href: '/documentations-pages', icon: 'user-circle-outline' },
    { name: 'Typography', href: '/typography-pages', icon: 'user-circle-outline' },
    { name: 'Colors', href: '/colors-pages', icon: 'user-circle-outline' }
  ];
  let name = "</>";
  let btnClass = 'text-gray-500 dark:text-gray-400 hover:bg-gray-100 dark:hover:bg-gray-700 rounded-lg text-xl p-2 md:p-0';
</script>

<Navbar let:hidden let:toggle class="bg-slate-100 dark:bg-gray-800 p-2 dark:border-slate-600 border-b border-slate-400 font-mono">
  <NavBrand href="/">
    <span class="self-center whitespace-nowrap text-2xl font-extrabold text-orange-400">{name}</span>
  </NavBrand>
    <DarkMode {btnClass}/>
</Navbar>