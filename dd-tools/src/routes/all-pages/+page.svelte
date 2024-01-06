<script>
    import { Card } from 'flowbite-svelte';
    import { Footer, FooterCopyright, FooterLinkGroup, FooterBrand, FooterLink } from 'flowbite-svelte';
    import { Popover, Button, Avatar } from 'flowbite-svelte';
    import Profile from "$lib/assets/profile.jpg";
    import Figma from "$lib/assets/figma.png";
    import Wireframe from  "$lib/assets/wireframe.png";
    import Photoshop from  "$lib/assets/photoshop.png";
    import Canva from  "$lib/assets/canva.png";
    import Sketch from  "$lib/assets/sketch.png";
    import Webflow from  "$lib/assets/webflow.png";
    import React from "$lib/assets/react.png";
    import Angular from "$lib/assets/angular.png";
    import Vue from  "$lib/assets/vue.png";
    import Sveltekit from  "$lib/assets/svelte.png";
    import Tailwind from  "$lib/assets/tailwind.png";
    import Bootstrap from  "$lib/assets/bootstrap.png";
    import Bulma from  "$lib/assets/bulma.png";
    import Nextjs from  "$lib/assets/nextjs.png";
    import Ember from  "$lib/assets/ember-logo.svg";
    import Express from "$lib/assets/Express.png";
    import Django from "$lib/assets/django.png";
    import Flask from  "$lib/assets/flask.png";
    import Rails from  "$lib/assets/rails.png";
    import Spring from  "$lib/assets/springboot.png";
    import Laravel from  "$lib/assets/laravel.png";
    import Net from  "$lib/assets/net.jpg";
    import Nest from  "$lib/assets/nestjs.png";
    import Fast from  "$lib/assets/fast.png";
    import Odin from "$lib/assets/Odin.png";
    import Scrimba from "$lib/assets/scrimba.png";
    import Udemy from "$lib/assets/Udemy.png";
    import CS50 from  "$lib/assets/CS50.png";
    import CodeCademy from  "$lib/assets/codecademy.png";
    import Khan from  "$lib/assets/Khan.png";
    import Coursera from  "$lib/assets/Coursera.png";
    import Free from  "$lib/assets/Free.png";
    import Sring from  "$lib/assets/sprintboard.png";
    import Mdn from "$lib/assets/mdn.png";
    import Wschool from "$lib/assets/w3.png";
    import Stack from "$lib/assets/stack.png";
    import Github from "$lib/assets/Github.png";
    import Glass from "$lib/assets/glass.png";
    import Google from "$lib/assets/google.png";
    import Flaticon from "$lib/assets/flaticon.png";
    import Finder from "$lib/assets/finder.png";
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
<div class="flex justify-center mt-16 lg:text-4xl md:text-2xl text-lg dark:text-slate-50 font-semibold">All tools, courses and more ⚙️<div class="lg:p-3 p-2 "><ChevronDownSolid class="lg:w-5 lg:h-5 w-4 h-4 text-black dark:text-white"/>
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
<div class="max-w-screen-lg m-auto grid md:grid-cols-3 gap-6 mt-16 justify-center md:grid-cols-2 lg:grid-cols-3">  
    <Card href="https://www.figma.com/" class="col-span-1" >
        <img src={Figma} alt="Figma" class="w-14 h-14">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Figma</h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Figma is a collaborative design tool in the cloud, allowing users to create, prototype, and iterate on interface designs seamlessly.</p>
    </Card>

    <Card href="https://www.adobe.com/products/photoshop.html" class="col-span-1" >
        <img src={Photoshop} alt="Adobe Photoshop" class="w-14 h-14">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Adobe Photoshop</h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            Adobe Photoshop is a versatile raster graphics editing software used for tasks like photo editing, graphic design, and digital art creation.</p>
    </Card>
    <Card href="https://www.canva.com/en_ph/" class="col-span-1" >
        <img src={Canva} alt="Canva" class="w-14 h-14">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Canva</h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight text-sm">Canva is a user-friendly online graphic design platform for creating a variety of visual content, from social media graphics to presentations.</p>
    </Card>

    <Card href="https://zeplin.io/" class="col-span-1" >
        <img src="https://cdn.sanity.io/images/wd3e2pma/production/7b336dc26fd85ae98b414761d58238d225876a88-60x48.svg" alt="Zeplin" class="w-14 h-14">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Zeplin</h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Zeplin is a design collaboration and handoff tool that streamlines communication between designers and developers by providing a platform for sharing and implementing design specifications.</p>
    </Card>

    <Card href="https://www.drawio.com/" class="col-span-1" >
        <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAHcAAAB3CAMAAAAO5y+4AAAAllBMVEXwhwXfbAz////dYQDwxK/fagDhbwvwhQD97ePwgwDwhxD+8+r//vzifkbxlEjxjijgcSHkhkvvfAD2uofvvaTki1voegndXQD34NTrfwfkdAr75NP3w5niezz89O/118jnmW/tsZL1rnT0qmrxlDz5zav51r7ym0/2vZHxo2nhdjTxjjbpoHvjg1DcVQD1s3zrqIfmlGU7M8bdAAADoUlEQVRoge3b2VriMBQA4JAQQ6AOEpZ2rJYWFRUZxfd/ubFDygfN3iZ0LnouwfTnZOtJEQBhupkScL0g400KIYAPjF6T/YEpe4AgZVdFj8FS8EQ7cOkGjDtgAZl2oZZwR24fffwfQeQRGGV0LA/KAu579PklHSli+xoMpm9QFy+B7mv0QcuWcAiW/DKwEL6HgNnW6Cb3/lkyHhndbPfbvzudGN3oFnuHLd2Bb9jW9Q1bu55he9cv7OB6hV1cn7CT6xF2c/3Bju5NR6432NX1BTu7nmB31w/cwPUCN3F9wI1cD3Aztz1sU+dEj4LbHqap0U1EdjBoW+vRJ6N7QBK3PWwqZKXptocJ0Pd0cqdwW8Nsrp7TkwKpWA9d/cGV/bKKnL/yRzq2nmDG19L6E1cRD48vZZ86tx1Mv3hyZyOJB9HxtUKbcBuYUE4szgl04B9moB7fMlbN033hU+gSQLzzt/qEG8P0mSeWXwL4u5pa+oSbwtW+sa7nFfM3EkPCzWC6OV49EtLCu+z4lnyfbAef7kdD8eKo4GtJuWNV4V5WszfdtavPFBtcZ5h8RJq+RNXUmpkSdoWZfu6gNX/bmLAbfLr5KhLCu2rjNk0tN5ipJxVPeMGH39jRLjCdG/fCmK+lhbmnrWEyNu/9eM+X985fxoxvzJkulzjh25lFwnYwOW3MulTwjP/V0iJhq+qWpVaLpKoAJhYJ27jVGpJV5RcJW1YAli6htjPVtgJQuYSeB+OPuzOEsHZ8Maqm1jBG5yFpJXEJe/2an8Ub773t/rC/jVUyjh/3hwMfYThcnEWRi7Lo0tcRhyQRrRWrE+/W6lYw+66PuODSd3Xzf5cQj5ol+2g4pNbvYnX3tFSVMZJOmsTUbKZ/AmHxJYLkBlztkZqoFWU11+ZQL7kDx8Z0YXY5Mequ+buan44W8zU/CoDaR0w27kQssGzcWet8e7d3e7d3e7d3e7cDt856cIPVV5G2vrKpJyWnLtS2nrSon2XPr/DA2NG1Q7F4Xpjr20fSUzWeaU4pZdQ7SXI+es807RPpMaU8qOiGOBOeLknOg3SVL4byKJbK7y4wWhaKVov8TpwSogvACqlCe/5Vt5I0k7lgpbm8p5C6V4DlbnhY4QaHVW5oWOkGhtVuWFjjBoV1bkhY6waE9W442OAGg01uKNjogvuO3DCwzS9FQsBg3Al8AzY2/6PtG8a55e+tPMNxYvv7Mp8wjgsIyt/TXXeMb/Kfmvcv2Jhhu6NnRC4AAAAASUVORK5CYII=" alt="Draw IO" class="w-14 h-14">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Draw IO</h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
          Draw IO is a web-based tool for creating diagrams, flowcharts, and visual representations. It's widely used for its user-friendly interface and collaborative features.</p>
    </Card>

    <Card href="https://www.sketch.com/" class="col-span-1" >
      <img src={Sketch} alt="sketch" class="w-14 h-14">
      <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Sketch</h5>
      <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
        Sketch is a design software for creating user interfaces, known for its intuitive interface and focus on user experience design.</p>
    </Card>

    <Card href="https://www.framer.com/" class="col-span-1" >
        <img src="https://th.bing.com/th?id=ODLS.804f77d1-b30b-4608-b167-d735609e91fe&w=32&h=32&qlt=90&pcl=fffffa&o=6&pid=1.2" alt="Framer X" class="w-14 h-14">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Framer X</h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
            Framer is a design and prototyping tool that empowers designers to create interactive user interfaces with a focus on dynamic user experiences.</p>
    </Card>

    <Card href="https://webflow.com/?r=0" class="col-span-1" >
      <img src={Webflow} alt="Webflow" class="w-14 h-14">
      <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Webflow</h5>
      <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
        Webflow is a visual web design and development platform, allowing users to create responsive websites without coding.</p>
    </Card>

    <Card href="https://wireframe.cc/" class="col-span-1" >
    <img src={Wireframe} alt="Wireframe" class="w-14 h-14">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Wireframe CC</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
      Wireframe.cc is an app that lets you create wireframes for any screen with a limited palette of colors and options.</p>
    </Card>
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
<Card href="https://www.theodinproject.com/" class="col-span-1" >
  <img src={Odin} alt="Odin Project" class="w-14 h-14">
  <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Odin Project</h5>
  <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">The Odin Project is a free web development curriculum for learning programming, HTML, CSS, and JavaScript through hands-on projects.</p>
</Card>

<Card href="https://cs50.harvard.edu/x/2024/" class="col-span-1" >
  <img src={CS50} alt="CS50" class="w-14 h-14">
  <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">CS50</h5>
  <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">CS50 is an introductory computer science course offered by Harvard University, covering fundamental concepts and programming languages.</p>
</Card>

<Card href="https://www.freecodecamp.org/" class="col-span-1" >
  <img src={Free} alt="FreeCodeCamp" class="w-14 h-14">
  <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">FreeCodeCamp</h5>
  <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
   freeCodeCamp is a nonprofit online platform offering free coding education, with interactive lessons and projects focusing on web development skills.</p>
</Card>
<Card href="https://www.codecademy.com/" class="col-span-1" >
  <img src={CodeCademy} alt="Code Cademy" class="w-16 h-16">
  <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">CodeCademy</h5>
  <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight text-sm">Codecademy is an online learning platform that offers interactive coding lessons to help users acquire programming skills.</p>
</Card>

<Card href="https://spring.io/" class="col-span-1" >
  <img src={Udemy} alt="Springboot" class="w-20 h-14">
  <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Udemy</h5>
  <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Udemy is an online learning platform offering a wide range of courses on various subjects, including programming, business, and personal development.</p>
</Card>

<Card href="https://www.khanacademy.org/" class="col-span-1" >
  <img src={Khan} alt="Khan Academy" class="w-14 h-14">
  <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Khan Academy</h5>
  <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
   Khan Academy is a non-profit educational platform offering free online courses in subjects like mathematics, science, and programming.</p>
</Card>

<Card href="https://www.coursera.org/" class="col-span-1" >
  <img src={Coursera} alt="ASP.NET" class="w-14 h-14">
  <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Coursera</h5>
  <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
   Coursera is an online learning platform that offers a variety of courses, certificates, and degree programs from universities and organizations worldwide.</p>
</Card>

<Card href="https://www.springboard.com/" class="col-span-1" >
  <img src={Sring} alt="Spring Board" class="w-14 h-14">
  <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Spring Board</h5>
  <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
   Springboard is an online platform for career-focused courses and mentorship programs.</p>
</Card>

<Card href="https://scrimba.com/" class="col-span-1" >
  <img src={Scrimba} alt="Scrimba" class="w-14 h-14">
  <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Scrimba</h5>
  <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
   Scrimba is an online learning platform that provides interactive coding tutorials using video playback and coding directly in the browser.</p>
</Card>
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

<Card href="https://fonts.google.com/" class="col-span-1" >
  <img src="https://designresourc.es/assets/image/5ea6cf3ffa94701139df77e0_5ea4d315d3a80f6efdc6df29_logo%20(25).png" alt="Google Fonts" class="w-14 h-14">
  <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Google Fonts</h5>
  <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Google Fonts is a free library of web fonts available for websites.</p>
</Card>

<Card href="https://www.typographicposters.com/?ref=designresourc.es" class="col-span-1" >
<img src="https://designresourc.es/assets/image/5ea4d840c07d784add385c0c_barra-220x220b_400x400.png"  alt="Typo/graphic" class="w-14 h-14">
<h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Typo/graphic</h5>
<p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
  Typographic is a platform for discovering and using typography in design projects.</p>
</Card>

<Card href="https://www.fontfabric.com/free-fonts/?ref=designresourc.es" class="col-span-1" >
  <img src="https://designresourc.es/assets/image/5ea6cb06925f489ed6077d5f_5ea4dc5a7899693e15cab57e_yAlEkZei_400x400.png" alt="Font fabric" class="w-14 h-14">
  <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Font fabric</h5>
  <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">FontFabric is a type foundry offering a variety of fonts for design use.</p>
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