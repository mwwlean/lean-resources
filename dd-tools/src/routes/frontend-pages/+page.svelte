<script>
    import { Card } from 'flowbite-svelte';
    import { Footer, FooterCopyright, FooterLinkGroup, FooterBrand, FooterLink } from 'flowbite-svelte';
    import { Popover, Button, Avatar } from 'flowbite-svelte';
 </script>
 
 <div class="flex justify-center mt-16 text-4xl dark:text-slate-50 font-semibold">FrontEnd Libraries and Tools 💻</div>
 <div class="max-w-screen-lg m-auto grid md:grid-cols-3 gap-6 mt-16 justify-center">  
        <Card href="/cards" class="col-span-1" >
            <img src="/src/routes/components/images/react.png" alt="ReactJS" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">ReactJs</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">React is an open-source JavaScript library by Facebook for building reusable and dynamic user interfaces in web applications.</p>
        </Card>
        
        <Card href="/cards" class="col-span-1" >
            <img src="/src/routes/components/images/angular.png" alt="Angular" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Angular</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Angular is an open-source web application framework by Google, using TypeScript, for building dynamic and scalable single-page applications.</p>
        </Card>
        
        <Card href="https://www.adobe.com/products/photoshop.html" class="col-span-1" >
            <img src="/src/routes/components/images/vue.png" alt="VueJS" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Vue</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
                Vue.js (Vue) is a lightweight and adaptable open-source JavaScript framework for building user interfaces, known for its simplicity and flexibility.</p>
        </Card>
        <Card href="/cards" class="col-span-1" >
            <img src="/src/routes/components/images/svelte.png" alt="sveltekit" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">SvelteKit</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight text-sm">SvelteKit is a framework extending Svelte, offering streamlined tools for building web applications with features like routing and server-side rendering.</p>
        </Card>
        
        <Card href="/cards" class="col-span-1" >
            <img src="/src/routes/components/images/tailwind.png" alt="tailwindCSS" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Tailwind CSS</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Tailwind CSS is a utility-first framework that streamlines web development with a customizable set of pre-built utility classes for styling HTML elements.</p>
        </Card>
        
        <Card href="https://www.adobe.com/products/photoshop.html" class="col-span-1" >
            <img src="/src/routes/components/images/bootstrap.png" alt="Bootstrap" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Bootstrap</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
                Bootstrap is a popular front-end framework that provides pre-designed HTML, CSS, and JavaScript components for building responsive and visually appealing websites and web applications.</p>
        </Card>
      
 </div>


 <Footer>
    <div class="flex justify-center m-auto my-16 ">
<p class="text-xs  dark:text-slate-50 tracking-tight">Created with SvelteKit and TailwindCSS by <span><a class="text-orange-400 font-bold underline" href="https://github.com/mwwlean" id="b2">mwwlean@github 🤠</a></span></p></div>
</Footer>
<Popover triggeredBy="#b2" class="w-64 text-sm font-light text-gray-500 bg-white dark:text-gray-400 dark:border-gray-600 dark:bg-gray-800">
<div class="p-3">
  <div class="flex justify-between items-center mb-2">
    <Avatar href="https://github.com/mwwlean" src="/src/routes/components/images/profile.jpg" alt="mwwlean" />
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