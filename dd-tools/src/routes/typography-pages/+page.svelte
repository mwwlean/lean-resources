<script>
    import { Card } from 'flowbite-svelte';
    import { Footer, FooterCopyright, FooterLinkGroup, FooterBrand, FooterLink } from 'flowbite-svelte';
    import { Popover, Button, Avatar } from 'flowbite-svelte';
    import Profile from "$lib/assets/profile.jpg";
    import { Dropdown, DropdownItem } from 'flowbite-svelte';
    import { ChevronDownSolid } from 'flowbite-svelte-icons';
    import { page } from '$app/stores';
    $: activeUrl = $page.url.pathname;
    export let buttonVisibleOnPX = 200;
    let hidden = true;

    const goStart = () => {
        window.scrollTo({
            top: 0,
            behavior: 'smooth'
        });
    };

    const scrollElement = () => {
        return document.documentElement || document.body;
    };

    const handleOnScroll = () => {
        if (scrollElement().scrollTop > buttonVisibleOnPX) {
            hidden = false;
        } else {
            hidden = true;
        }
    };
 </script>
 
 <svelte:window on:scroll={handleOnScroll} />
 <div class="back_to_start" on:click={goStart} class:hidden>☝🏻☝🏻☝🏻</div>
 <div class="flex justify-center mt-16 lg:text-4xl md:text-2xl text-xl dark:text-slate-50 font-semibold">Typography 🗚<div class="lg:p-3 p-2"><ChevronDownSolid class="lg:w-5 lg:h-5 w-4 h-4 text-black dark:text-white"/>
  <Dropdown {activeUrl}>
    <DropdownItem href="/all-pages">All</DropdownItem>
    <DropdownItem href="/design-pages">Design</DropdownItem>
    <DropdownItem href="/frontend-pages">Frontend Tools</DropdownItem>
    <DropdownItem href="/backend-pages">Backend Tools</DropdownItem>
    <DropdownItem href="/courses-pages">Coding Courses</DropdownItem>
    <DropdownItem href="/documentations-pages">Documentations</DropdownItem>
    <DropdownItem href="/icons-pages">Icons</DropdownItem>
    <DropdownItem href="/colors-pages">Colors</DropdownItem>
    <DropdownItem href="/typography-pages">Typography</DropdownItem>

  </Dropdown></div>
</div>
 <div class="max-w-screen-lg m-auto grid md:grid-cols-2 lg:grid-cols-3 gap-6 mt-16 justify-center">  
        <Card href="https://fonts.google.com/" class="col-span-1" >
            <img src="https://designresourc.es/assets/image/5ea6cf3ffa94701139df77e0_5ea4d315d3a80f6efdc6df29_logo%20(25).png" alt="Google Fonts" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Google Fonts</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Google Fonts is a free library of web fonts available for websites.</p>
        </Card>

        <Card href="https://www.typographicposters.com/?ref=designresourc.es" class="col-span-1" >
          <img src="https://designresourc.es/assets/image/5ea4d840c07d784add385c0c_barra-220x220b_400x400.png"  alt="Typo/graphic" class="w-14 h-14">
          <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Typo/graphic</h5>
          <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            Typographic is a platform for discovering and using typography in design projects.</p>
      </Card>
        
        <Card href="https://www.fontfabric.com/free-fonts/?ref=designresourc.es" class="col-span-1" >
            <img src="https://designresourc.es/assets/image/5ea6cb06925f489ed6077d5f_5ea4dc5a7899693e15cab57e_yAlEkZei_400x400.png" alt="Font fabric" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Font fabric</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">FontFabric is a type foundry offering a variety of fonts for design use.</p>
        </Card>
     
 </div>


 <Footer>
    <div class="flex justify-center m-auto my-16 ">
      <p class="text-xs  dark:text-slate-50 tracking-tight">Created with SvelteKit and TailwindCSS by <span><a class="text-orange-400 font-bold underline" href="https://github.com/mwwlean" id="b2">mwwlean@github 🤠</a></span></p></div>
 </Footer>
    <Popover triggeredBy="#b2" class="w-64 text-sm font-light text-gray-500 bg-white dark:text-gray-400 dark:border-gray-600 dark:bg-gray-800">
      <div class="p-3">
        <div class="flex justify-between items-center mb-2">
          <Avatar href="https://github.com/mwwlean" src={Profile} alt="mwwlean" />
            <a href="https://github.com/mwwlean"><Button size="xs">View Github Profile</Button></a> 
        </div>
        <div class="text-base font-semibold leading-none text-gray-900 dark:text-white">
          <a href="/">leander</a>
        </div>

        <div class="mb-4 text-sm font-light pt-2">
        UI Designer & Developer at <a href="https://www.cenixys.com/" class="text-primary-600 dark:text-primary-500 hover:underline"> cenixys.com </a>
        </div>
        <ul class="flex text-sm font-light">
          <li class="me-2">
            <a href="https://github.com/mwwlean?tab=following" class="hover:underline">
              <span class="font-semibold text-gray-900 dark:text-white">8</span>
              <span>Following</span>
            </a>
          </li>
          <li>
            <a href="https://github.com/mwwlean?tab=followers" class="hover:underline">
              <span class="font-semibold text-gray-900 dark:text-white">7</span>
              <span>Followers</span>
            </a>
          </li>
        </ul>
      </div>
</Popover>

<style>
  .back_to_start {
        opacity: 1;
        transition: opacity 0.5s, visibility 0.5s;
        position: fixed;
        z-index: 99;
        right: 20px;
        user-select: none;
        bottom: 20px;
        color: white;
        background-color: rgb(255, 98, 0);
        padding: 5px;
        font-weight: 700;
        border-radius: 5px;
    }
    
    .back_to_start.hidden {
        opacity: 0;
        visibility: hidden;
    }
</style>