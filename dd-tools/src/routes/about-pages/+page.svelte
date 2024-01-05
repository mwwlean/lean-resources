<script>
    import { Card } from 'flowbite-svelte';
   import { Footer, FooterCopyright, FooterLinkGroup, FooterBrand, FooterLink } from 'flowbite-svelte';
   import { Popover, Button, Avatar } from 'flowbite-svelte';
   import Profile from "$lib/assets/profile.jpg";
   import Express from "$lib/assets/Express.png";
   import Django from "$lib/assets/django.png";
   import Flask from  "$lib/assets/flask.png";
   import Rails from  "$lib/assets/rails.png";
   import Spring from  "$lib/assets/springboot.png";
   import Laravel from  "$lib/assets/laravel.png";
   import Net from  "$lib/assets/net.jpg";
   import Nest from  "$lib/assets/nestjs.png";
   import Fast from  "$lib/assets/fast.png";
</script>

<div class="flex justify-center mt-16 lg:text-4xl md:text-2xl text-xl dark:text-slate-50 font-semibold">Choose</div>
<div class="max-w-screen-lg m-auto grid md:grid-cols-3 gap-6 mt-16 justify-center md:grid-cols-2 lg:grid-cols-3">  
       <Card href="https://expressjs.com/" class="col-span-1" >
           <img src={Express} alt="ExpressJS" class="w-14 h-14">
           <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Express.js</h5>
           <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Express.js is a lightweight framework for building web applications and APIs in Node.js, known for its simplicity and flexibility.</p>
       </Card>
       
       <Card href="https://www.djangoproject.com/" class="col-span-1" >
           <img src={Django} alt="Django" class="w-14 h-14">
           <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Django</h5>
           <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Django is a high-level Python web framework, simplifying web development with built-in features for creating robust and scalable applications.</p>
       </Card>
       
       <Card href="https://flask.palletsprojects.com/en/3.0.x/" class="col-span-1" >
           <img src={Flask} alt="Flask" class="w-14 h-14">
           <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Flask</h5>
           <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
               Flask is a lightweight Python web framework, providing simplicity and flexibility for building web applications with minimal boilerplate code.</p>
       </Card>
       <Card href="https://rubyonrails.org/" class="col-span-1" >
           <img src={Rails} alt="Ruby on rails" class="w-14 h-14">
           <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Ruby on Rails</h5>
           <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight text-sm">Ruby on Rails (Rails) is a full-stack web framework written in Ruby, known for its convention-over-configuration approach and built-in tools for efficient web development.</p>
       </Card>
       
       <Card href="https://spring.io/" class="col-span-1" >
           <img src={Spring} alt="Springboot" class="w-14 h-14">
           <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Spring Boot</h5>
           <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Spring Boot is a Java-based framework that simplifies building production-ready applications by providing conventions and an embedded web server for ease of development.</p>
       </Card>
       
       <Card href="https://laravel.com/" class="col-span-1" >
           <img src={Laravel} alt="Laravel" class="w-14 h-14">
           <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Laravel</h5>
           <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
               Laravel is a PHP web framework, recognized for its elegant syntax and expressive features, streamlining the development of modern and scalable web applications.</p>
       </Card>

       <Card href="https://dotnet.microsoft.com/en-us/apps/aspnet" class="col-span-1" >
           <img src={Net} alt="ASP.NET" class="w-14 h-14">
           <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">ASP.NET</h5>
           <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
               ASP.NET is a web application framework by Microsoft, supporting multiple languages and facilitating the development of dynamic and scalable web applications.</p>
       </Card>

       <Card href="https://nestjs.com/" class="col-span-1" >
           <img src={Nest} alt="Nest JS" class="w-14 h-14">
           <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Nest.js</h5>
           <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
               Nest.js is a Node.js framework for building scalable server-side applications with TypeScript and a modular structure.</p>
       </Card>

       <Card href="https://fastapi.tiangolo.com/" class="col-span-1" >
           <img src={Fast} alt="Fast API" class="w-14 h-14">
           <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">FastAPI</h5>
           <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
               FastAPI is a high-performance Python web framework for building APIs, known for its ease of use, efficiency, and automatic validation and documentation features.</p>
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