<script>
    import { Card } from 'flowbite-svelte';
    import { Footer, FooterCopyright, FooterLinkGroup, FooterBrand, FooterLink } from 'flowbite-svelte';
    import { Popover, Button, Avatar } from 'flowbite-svelte';
    import Profile from "$lib/assets/profile.png";
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
 <div class="flex justify-center mt-16 lg:text-4xl md:text-2xl text-xl dark:text-slate-50 font-semibold">Colors 🎨<div class="lg:p-3 p-2"><ChevronDownSolid class="lg:w-5 lg:h-5 w-4 h-4 text-black dark:text-white"/>
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
 <div class="max-w-screen-lg m-auto grid md:grid-cols-2 lg:grid-cols-3 gap-6 mt-16 justify-center animate-fade-right animate-once animate-duration-[800ms] animate-delay-200 animate-ease-in-out animate-normal">  
        <Card href="https://www.khroma.co/" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
            <img src="https://designresourc.es/assets/image/5ea6cf69a13e986dd80ffa3f_5ea1af0ffe57820563564805_logo%20(1).png" alt="Khroma" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Khroma</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Khroma is a tool for generating color palettes based on your preferences.</p>
        </Card>

        <Card href="https://colorhunt.co/?ref=designresourc.es" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
          <img src="https://designresourc.es/_next/image?url=%2Fimg%2F5ea0291287be017411f4dc60_colorhunt.jpg&w=48&q=75"  alt="Color hunt" class="w-14 h-14">
          <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Color hunt</h5>
          <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            Color Hunt is a website providing curated color palettes for design inspiration.</p>
      </Card>
        
        <Card href="https://pigment.shapefactory.co/?ref=designresourc.es" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
            <img src="https://designresourc.es/_next/image?url=%2Fimg%2F5ea6cf67fadd3cd93ad57b61_5ea1c171b910a3ad1dca6c08_logo%2520(3).png&w=48&q=75" alt="Pigment" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Pigment</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Pigment is an app for creating and exploring color palettes, widely used for design inspiration.</p>
        </Card>
     
        <Card href="https://coolors.co/?ref=designresourc.es" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
            <img src="https://designresourc.es/_next/image?url=%2Fimg%2F5ebff9260962176e64a111c1_Coolors.jpg&w=48&q=75" alt="Coolers" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Coolors</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Coolors is a color scheme generator for creating harmonious palettes.</p>
        </Card>

        <Card href="https://www.culrs.com/?ref=designresourc.es" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
          <img src="https://designresourc.es/_next/image?url=%2Fimg%2F5ea6caee8b51eb51c9eae398_5ea59b89f0e208f92353b922_2980900f-ddbe-406b-a188-ed1f7fcc1d52.gif&w=48&q=75"  alt="Curls" class="w-14 h-14">
          <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Curls</h5>
          <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            Culrs is a simple tool for creating color palettes.</p>
      </Card>
        
        <Card href="https://www.happyhues.co/" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
            <img src="https://designresourc.es/_next/image?url=%2Fimg%2F5ea592f8c07d78e3663ba689_f7e1dd94-a807-44ba-adb0-8482164a0a0b.gif&w=48&q=75" alt="Happy Hues" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Happy Hues</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Happy Hues is a website offering beautiful color combinations for design.</p>
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
              <span class="font-semibold text-gray-900 dark:text-white">12</span>
              <span>Following</span>
            </a>
          </li>
          <li>
            <a href="https://github.com/mwwlean?tab=followers" class="hover:underline">
              <span class="font-semibold text-gray-900 dark:text-white">8</span>
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