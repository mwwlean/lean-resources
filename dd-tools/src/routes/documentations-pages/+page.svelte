<script>
    import { Card } from 'flowbite-svelte';
    import { Footer, FooterCopyright, FooterLinkGroup, FooterBrand, FooterLink } from 'flowbite-svelte';
    import { Popover, Button, Avatar } from 'flowbite-svelte';
    import Profile from "$lib/assets/profile.jpg";
    import Flaticon from "$lib/assets/flaticon.png";
    import Finder from "$lib/assets/finder.png";

 </script>
 
 <div class="flex justify-center mt-16 lg:text-4xl md:text-2xl text-xl dark:text-slate-50 font-semibold">Icons  💻</div>
 <div class="max-w-screen-lg m-auto grid md:grid-cols-2 lg:grid-cols-3 gap-6 mt-16 justify-center">  
        <Card href="https://fontawesome.com/" class="col-span-1" >
            <img src="https://designresourc.es/assets/image/5ea6cf4e2fa37ecdf92c4d58_5ea4667e8ad6b62e139228cc_JqER8seZ_400x400.png" alt="Font Awesome" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Fontawesome</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">FontAwesome is a popular icon toolkit that provides a collection of scalable vector icons for web and application development.</p>
        </Card>

        <Card href="https://fonts.google.com/icons" class="col-span-1" >
          <img src="https://designresourc.es/assets/image/5ea6cf7013c0020120b0a1e9_5e9b7861572a494adcce5d74_google.png"  alt="Material Icons" class="w-14 h-14">
          <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Material Icons</h5>
          <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            Material Icons are a set of design-consistent icons created by Google for use in web and mobile applications.</p>
      </Card>
        
        <Card href="https://feathericons.com/" class="col-span-1" >
            <img src="https://designresourc.es/assets/image/5ea6cfa62fa37e32bd2ca95c_5e9b783638205aab56d08b62_feather.png" alt="Feather Icons" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Feather Icons</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Feather Icons is a collection of simple and customizable icons designed for web projects, offering a lightweight and clean aesthetic.</p>
        </Card>
        
        <Card href="https://ionic.io/ionicons/" class="col-span-1" >
            <img src="https://designresourc.es/assets/image/5ea6cfa7fadd3cf6d4d5ca73_5e9b78301b847f68844f9e05_ionicons.png" alt="Ionicons" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Ionicons</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
              Ionicons is a popular set of free and open-source icons designed for use in web, mobile, and desktop applications.</p>
        </Card>
        <Card href="https://icons8.com/icons" class="col-span-1" >
            <img src="https://designresourc.es/assets/image/5ea6cf712fa37e16e52c6bd7_5ea0aca1f1271e01b71e7e87_pMw2UlcW_400x400.jpeg" alt="Icons8" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Icons8</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight text-sm">Icons8 is a platform offering a wide variety of free icons for use in design projects, providing a searchable library of visuals in different styles and formats.</p>
        </Card>
        
        <Card href="https://www.streamlinehq.com/" class="col-span-1" >
          <img src="https://designresourc.es/assets/image/5f197caa77a6a13ee805e0eb_streamline.png"  alt="Streamline" class="w-16 h-14">
          <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Streamline</h5>
          <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            Streamline is a collection of customizable icons available for use in design projects, providing a diverse set of high-quality visuals in various styles.</p>
      </Card>

        <Card href="https://css.gg/" class="col-span-1" >
            <img src="https://designresourc.es/assets/image/5ea6cf40607f88bf2a46f2b1_5ea487f60e3498b2143435c6_logo%20(24).png" alt="CSS.GG" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">CSS.GG</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Open-source CSS, SVG and Figma UI Icons
              Available in SVG Sprite, styled-components, NPM & API</p>
        </Card>
        
        <Card href="https://www.flaticon.com/search?word=angular" class="col-span-1" >
            <img src={Flaticon}  alt="Flaticon" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Flaticon</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
              Flaticon is a platform providing a vast collection of free and customizable vector icons for use in design projects, offering a diverse range of styles and categories.</p>
        </Card>
        <Card href="https://www.iconfinder.com/" class="col-span-1" >
          <img src={Finder}  alt="Icon Finder" class="w-14 h-14">
          <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Icon Finder</h5>
          <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            Iconfinder is a platform offering a diverse collection of icons for use in design projects, providing a searchable library of high-quality icons in various styles and formats.</p>
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