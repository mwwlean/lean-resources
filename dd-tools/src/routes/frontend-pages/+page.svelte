<script>
    import { Card } from 'flowbite-svelte';
    import { Footer, FooterCopyright, FooterLinkGroup, FooterBrand, FooterLink } from 'flowbite-svelte';
    import { Popover, Button, Avatar } from 'flowbite-svelte';
    import Profile from "$lib/assets/profile.jpg";
    import React from "$lib/assets/react.png";
    import Angular from "$lib/assets/angular.png";
    import Vue from  "$lib/assets/vue.png";
    import Sveltekit from  "$lib/assets/svelte.png";
    import Tailwind from  "$lib/assets/tailwind.png";
    import Bootstrap from  "$lib/assets/bootstrap.png";
    import Bulma from  "$lib/assets/bulma.png";
    import Nextjs from  "$lib/assets/nextjs.png";
    import Ember from  "$lib/assets/ember-logo.svg";
 </script>
 
 <div class="flex justify-center mt-16 lg:text-4xl md:text-2xl text-xl dark:text-slate-50 font-semibold">Frontend Frameworks and Tools 💻</div>
 <div class="max-w-screen-lg m-auto grid md:grid-cols-2 lg:grid-cols-3 gap-6 mt-16 justify-center">  
        <Card href="https://react.dev/" class="col-span-1" >
            <img src={React} alt="ReactJS" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">React</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">React is an open-source JavaScript library by Facebook for building reusable and dynamic user interfaces in web applications.</p>
        </Card>

        <Card href="https://nextjs.org/" class="col-span-1" >
          <img src={Nextjs}  alt="Nextjs" class="w-14 h-14">
          <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">NextJs</h5>
          <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            Next.js is a React-based framework for building modern web applications with features like server-side rendering and automatic code splitting.</p>
      </Card>
        
        <Card href="https://angularjs.org/" class="col-span-1" >
            <img src={Angular} alt="Angular" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Angular</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Angular is an open-source web application framework by Google, using TypeScript, for building dynamic and scalable single-page applications.</p>
        </Card>
        
        <Card href="https://vuejs.org/" class="col-span-1" >
            <img src={Vue} alt="VueJS" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Vue</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
                Vue.js (Vue) is a lightweight and adaptable open-source JavaScript framework for building user interfaces, known for its simplicity and flexibility.</p>
        </Card>
        <Card href="https://kit.svelte.dev/ " class="col-span-1" >
            <img src={Sveltekit} alt="sveltekit" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">SvelteKit</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight text-sm">SvelteKit is a framework extending Svelte, offering streamlined tools for building web applications with features like routing and server-side rendering.</p>
        </Card>
        
        <Card href="https://emberjs.com/" class="col-span-1" >
          <img src="{Ember}"  alt="EmberJS" class="w-20 h-14">
          <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">EmberJs</h5>
          <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            Ember.js is an open-source JavaScript framework for building scalable web applications with a strong emphasis on convention and productivity.</p>
      </Card>

        <Card href="https://tailwindcss.com/" class="col-span-1" >
            <img src={Tailwind} alt="tailwindCSS" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Tailwind CSS</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Tailwind CSS is a utility-first framework that streamlines web development with a customizable set of pre-built utility classes for styling HTML elements.</p>
        </Card>
        
        <Card href="https://getbootstrap.com/" class="col-span-1" >
            <img src={Bootstrap}  alt="Bootstrap" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Bootstrap</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
              Bootstrap is a widely-used front-end framework with pre-designed HTML, CSS, and JavaScript components for creating responsive websites and web applications.</p>
        </Card>
        <Card href="https://bulma.io/" class="col-span-1" >
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