<script>
    import { Card } from 'flowbite-svelte';
    import { Footer, FooterCopyright, FooterLinkGroup, FooterBrand, FooterLink } from 'flowbite-svelte';
    import { Popover, Button, Avatar } from 'flowbite-svelte';
    import Profile from "$lib/assets/profile.png";
    import React from "$lib/assets/react.png";
    import Angular from "$lib/assets/angular.png";
    import Vue from  "$lib/assets/vue.png";
    import Sveltekit from  "$lib/assets/svelte.png";
    import Tailwind from  "$lib/assets/tailwind.png";
    import Bootstrap from  "$lib/assets/bootstrap.png";
    import Bulma from  "$lib/assets/bulma.png";
    import Nextjs from  "$lib/assets/nextjs.png";
    import Ember from  "$lib/assets/ember-logo.svg";
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
 <div class="flex justify-center mt-16 lg:text-4xl md:text-2xl text-xl dark:text-slate-50 font-semibold">Frontend Frameworks and tools💻<div class="lg:p-3 p-2"><ChevronDownSolid class="lg:w-5 lg:h-5 w-4 h-4 text-black dark:text-white"/>
  <Dropdown {activeUrl}>
    <DropdownItem href="/all-pages">All</DropdownItem>
    <DropdownItem href="/design-pages">Design</DropdownItem>
    <DropdownItem href="/frontend-pages">Frontend Tools</DropdownItem>
    <DropdownItem href="/backend-pages">Backend Tools</DropdownItem>
    <DropdownItem href="/courses-pages">Coding Courses</DropdownItem>
    <DropdownItem href="/documentatio-pages">Documentations</DropdownItem>
    <DropdownItem href="/icons-pages">Icons</DropdownItem>
    <DropdownItem href="/colors-pages">Colors</DropdownItem>
    <DropdownItem href="/typography-pages">Typography</DropdownItem>

  </Dropdown></div>
</div>
 <div class="max-w-screen-lg m-auto grid md:grid-cols-2 lg:grid-cols-3 gap-6 mt-16 justify-center animate-fade-right animate-once animate-duration-[800ms] animate-delay-200 animate-ease-in-out animate-normal">  
        <Card href="https://react.dev/" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
            <img src={React} alt="ReactJS" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">React</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">React is an open-source JavaScript library by Facebook for building reusable and dynamic user interfaces in web applications.</p>
        </Card>

        <Card href="https://nextjs.org/" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
          <img src={Nextjs}  alt="Nextjs" class="w-14 h-14">
          <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">NextJs</h5>
          <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            Next.js is a React-based framework for building modern web applications with features like server-side rendering and automatic code splitting.</p>
      </Card>
        
        <Card href="https://angularjs.org/" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
            <img src={Angular} alt="Angular" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Angular</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Angular is an open-source web application framework by Google, using TypeScript, for building dynamic and scalable single-page applications.</p>
        </Card>
        
        <Card href="https://vuejs.org/" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
            <img src={Vue} alt="VueJS" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Vue</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
                Vue.js (Vue) is a lightweight and adaptable open-source JavaScript framework for building user interfaces, known for its simplicity and flexibility.</p>
        </Card>
        <Card href="https://kit.svelte.dev/ " class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
            <img src={Sveltekit} alt="sveltekit" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">SvelteKit</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight text-sm">SvelteKit is a framework extending Svelte, offering streamlined tools for building web applications with features like routing and server-side rendering.</p>
        </Card>
        
        <Card href="https://emberjs.com/" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
          <img src="{Ember}"  alt="EmberJS" class="w-20 h-14">
          <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">EmberJs</h5>
          <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            Ember.js is an open-source JavaScript framework for building scalable web applications with a strong emphasis on convention and productivity.</p>
      </Card>

        <Card href="https://tailwindcss.com/" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
            <img src={Tailwind} alt="tailwindCSS" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Tailwind CSS</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Tailwind CSS is a utility-first framework that streamlines web development with a customizable set of pre-built utility classes for styling HTML elements.</p>
        </Card>
        
        <Card href="https://getbootstrap.com/" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
            <img src={Bootstrap}  alt="Bootstrap" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Bootstrap</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
              Bootstrap is a widely-used front-end framework with pre-designed HTML, CSS, and JavaScript components for creating responsive websites and web applications.</p>
        </Card>
        <Card href="https://bulma.io/" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
          <img src={Bulma}  alt="Bulma CSS" class="w-14 h-14">
          <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Bulma</h5>
          <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            Bulma is a modern, open-source CSS framework for creating responsive and flexible web designs with customizable components.</p>
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