<script>
    import { Card } from 'flowbite-svelte';
   import { Footer, FooterCopyright, FooterLinkGroup, FooterBrand, FooterLink } from 'flowbite-svelte';
   import { Popover, Button, Avatar } from 'flowbite-svelte';
   import Profile from "$lib/assets/profile.png";
   import Odin from "$lib/assets/Odin.png";
   import Scrimba from "$lib/assets/scrimba.png";
   import Udemy from "$lib/assets/Udemy.png";
   import CS50 from  "$lib/assets/CS50.png";
   import CodeCademy from  "$lib/assets/codecademy.png";
   import Khan from  "$lib/assets/Khan.png";
   import Coursera from  "$lib/assets/Coursera.png";
   import Free from  "$lib/assets/Free.png";
   import Sring from  "$lib/assets/sprintboard.png";
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
 <div class="flex justify-center mt-16 lg:text-4xl md:text-2xl text-xl dark:text-slate-50 font-semibold">Online Coding Courses 📚<div class="lg:p-3 p-2"><ChevronDownSolid class="lg:w-5 lg:h-5 w-4 h-4 text-black dark:text-white"/>
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
<div class="max-w-screen-lg m-auto grid md:grid-cols-3 gap-6 mt-16 justify-center md:grid-cols-2 lg:grid-cols-3 animate-fade-right animate-once animate-duration-[800ms] animate-delay-200 animate-ease-in-out animate-normal">  
       <Card href="https://www.theodinproject.com/" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
           <img src={Odin} alt="Odin Project" class="w-14 h-14">
           <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Odin Project</h5>
           <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">The Odin Project is a free web development curriculum for learning programming, HTML, CSS, and JavaScript through hands-on projects.</p>
       </Card>
       
       <Card href="https://cs50.harvard.edu/x/2024/" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
           <img src={CS50} alt="CS50" class="w-14 h-14">
           <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">CS50</h5>
           <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">CS50 is an introductory computer science course offered by Harvard University, covering fundamental concepts and programming languages.</p>
       </Card>
       
       <Card href="https://www.freecodecamp.org/" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
           <img src={Free} alt="FreeCodeCamp" class="w-14 h-14">
           <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">FreeCodeCamp</h5>
           <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            freeCodeCamp is a nonprofit online platform offering free coding education, with interactive lessons and projects focusing on web development skills.</p>
       </Card>
       <Card href="https://www.codecademy.com/" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
           <img src={CodeCademy} alt="Code Cademy" class="w-16 h-16">
           <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">CodeCademy</h5>
           <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight text-sm">Codecademy is an online learning platform that offers interactive coding lessons to help users acquire programming skills.</p>
       </Card>
       
       <Card href="https://spring.io/" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
           <img src={Udemy} alt="Springboot" class="w-20 h-14">
           <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Udemy</h5>
           <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Udemy is an online learning platform offering a wide range of courses on various subjects, including programming, business, and personal development.</p>
       </Card>
       
       <Card href="https://www.khanacademy.org/" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
           <img src={Khan} alt="Khan Academy" class="w-14 h-14">
           <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Khan Academy</h5>
           <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            Khan Academy is a non-profit educational platform offering free online courses in subjects like mathematics, science, and programming.</p>
       </Card>

       <Card href="https://www.coursera.org/" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
           <img src={Coursera} alt="ASP.NET" class="w-14 h-14">
           <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Coursera</h5>
           <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            Coursera is an online learning platform that offers a variety of courses, certificates, and degree programs from universities and organizations worldwide.</p>
       </Card>

       <Card href="https://www.springboard.com/" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
           <img src={Sring} alt="Spring Board" class="w-14 h-14">
           <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Spring Board</h5>
           <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            Springboard is an online platform for career-focused courses and mentorship programs.</p>
       </Card>

       <Card href="https://scrimba.com/" class="col-span-1  transition duration-500 ease-in-out transition-transform hover:scale-[1.1]" >
           <img src={Scrimba} alt="Scrimba" class="w-14 h-14">
           <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Scrimba</h5>
           <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            Scrimba is an online learning platform that provides interactive coding tutorials using video playback and coding directly in the browser.</p>
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