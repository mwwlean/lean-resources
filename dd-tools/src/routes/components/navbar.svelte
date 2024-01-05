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
  <NavHamburger on:click={toggle} />
  <NavUl {hidden}>
    <NavLi class="cursor-pointer lg:text-base font-normal" >
      Dev Tools<ChevronDownOutline class="w-3 h-3 ms-2 text-primary-800 dark:text-white inline" />
    </NavLi>
    <MegaMenu items={menu} let:item>
      <a href={item.href} class="flex items-center hover:text-primary-600 dark:hover:text-primary-500 lg:text-base font-normal">
        <span class="sr-only">{item.name}</span>
        <svelte:component this={IconOutline} name={item.icon} class="w-4 h-4 me-2" />{item.name}
      </a>
    </MegaMenu>
    <NavLi href="/about-pages"  class="lg:text-base font-normal"></NavLi>
    

    
    <DarkMode {btnClass}/>
  </NavUl>
</Navbar>