<script>
    import { Card } from 'flowbite-svelte';
    import { Footer, FooterCopyright, FooterLinkGroup, FooterBrand, FooterLink } from 'flowbite-svelte';
    import { Popover, Button, Avatar } from 'flowbite-svelte';
    import Profile from "$lib/assets/profile.jpg";
    import Mdn from "$lib/assets/mdn.png";
    import Wschool from "$lib/assets/w3.png";
    import Stack from "$lib/assets/stack.png";
    import Github from "$lib/assets/Github.png";
    import Glass from "$lib/assets/glass.png";
    import Google from "$lib/assets/google.png";

 </script>
 
 <div class="flex justify-center mt-16 lg:text-4xl md:text-2xl text-xl dark:text-slate-50 font-semibold">Documentations  📔</div>
 <div class="max-w-screen-lg m-auto grid md:grid-cols-2 lg:grid-cols-3 gap-6 mt-16 justify-center">  
        <Card href="https://developer.mozilla.org/en-US/" class="col-span-1" >
            <img src={Mdn} alt="MDN DOCUMENTATIONS" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">MDN</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">MDN (Mozilla Developer Network) is a resource for web developers with extensive documentation and guides.</p>
        </Card>

        <Card href="https://www.w3schools.com/" class="col-span-1" >
          <img src={Wschool}  alt="W3school" class="w-14 h-14">
          <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">W3Schools</h5>
          <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            W3Schools is an online learning platform offering web development tutorials and references.</p>
      </Card>
        
        <Card href="https://stackoverflow.com/" class="col-span-1" >
            <img src={Stack} alt="Stack Overflow" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Stack Overflow</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Stack Overflow is a Q&A platform where developers seek and share programming solutions.</p>
        </Card>
        
        <Card href="https://github.com/" class="col-span-1" >
            <img src={Github} alt="Github" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">GitHub</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
              GitHub Documentation is the official documentation for GitHub, a platform for version control and collaboration.</p>
        </Card>
        <Card href="https://devdocs.io/" class="col-span-1" >
            <img src={Glass} alt="Dev Docs" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">DevDocs</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight text-sm">DevDocs is a unified documentation platform aggregating documentation for various technologies.</p>
        </Card>

        <Card href="https://developer.mozilla.org/en-US/docs/Web/javascript" class="col-span-1" >
            <img src={Mdn} alt="Javascript MDN" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">JavaScript MDN</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">JavaScript MDN is the Mozilla Developer Network's documentation specifically for JavaScript.</p>
        </Card>
        
        <Card href="https://developers.google.com/" class="col-span-1" >
            <img src={Google} alt="Google Developers" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Google Developers</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
              Google Developers is Google's resource hub for developers, providing tools, documentation, and APIs.</p>
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
