<script>
    import { Card } from 'flowbite-svelte';
    import { Footer, FooterCopyright, FooterLinkGroup, FooterBrand, FooterLink } from 'flowbite-svelte';
    import { Popover, Button, Avatar } from 'flowbite-svelte';
    import Profile from "$lib/assets/profile.jpg";

 </script>
 
 <div class="flex justify-center mt-16 lg:text-4xl md:text-2xl text-xl dark:text-slate-50 font-semibold">Colors 🎨</div>
 <div class="max-w-screen-lg m-auto grid md:grid-cols-2 lg:grid-cols-3 gap-6 mt-16 justify-center">  
        <Card href="https://fonts.google.com/" class="col-span-1" >
            <img src="https://designresourc.es/assets/image/5ea6cf69a13e986dd80ffa3f_5ea1af0ffe57820563564805_logo%20(1).png" alt="Khroma" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Khroma</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Khroma is a tool for generating color palettes based on your preferences.</p>
        </Card>

        <Card href="https://www.typographicposters.com/?ref=designresourc.es" class="col-span-1" >
          <img src="https://designresourc.es/assets/image/5ea0291287be017411f4dc60_colorhunt-p-500.jpeg"  alt="Color hunt" class="w-14 h-14">
          <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Color hunt</h5>
          <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            Color Hunt is a website providing curated color palettes for design inspiration.</p>
      </Card>
        
        <Card href="https://www.fontfabric.com/free-fonts/?ref=designresourc.es" class="col-span-1" >
            <img src="https://designresourc.es/assets/image/5ea6cf67fadd3cd93ad57b61_5ea1c171b910a3ad1dca6c08_logo%20(3).png" alt="Font fabric" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Pigment</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Pigment is an app for creating and exploring color palettes, widely used for design inspiration.</p>
        </Card>
     
        <Card href="https://fonts.google.com/" class="col-span-1" >
            <img src="https://designresourc.es/assets/image/5ebff9260962176e64a111c1_Coolors.jpg" alt="Coolers" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Coolers</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Coolors is a color scheme generator for creating harmonious palettes.</p>
        </Card>

        <Card href="https://www.typographicposters.com/?ref=designresourc.es" class="col-span-1" >
          <img src="https://designresourc.es/assets/image/5ea6caee8b51eb51c9eae398_5ea59b89f0e208f92353b922_2980900f-ddbe-406b-a188-ed1f7fcc1d52.gif"  alt="Curls" class="w-14 h-14">
          <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Curls</h5>
          <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            Culrs is a simple tool for creating color palettes.</p>
      </Card>
        
        <Card href="https://www.fontfabric.com/free-fonts/?ref=designresourc.es" class="col-span-1" >
            <img src="https://designresourc.es/assets/image/5ea592f8c07d78e3663ba689_f7e1dd94-a807-44ba-adb0-8482164a0a0b.gif" alt="Happy Hues" class="w-14 h-14">
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