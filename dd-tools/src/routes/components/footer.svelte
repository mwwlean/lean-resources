<script>
    import { Footer, FooterCopyright, FooterLinkGroup, FooterBrand, FooterLink } from 'flowbite-svelte';
    import { Popover, Button, Avatar } from 'flowbite-svelte';
    import Profile from "$lib/assets/profile.png";
  </script>
 
    <Footer>
        <div class="flex justify-center m-auto">
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