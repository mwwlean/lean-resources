<script>
     import Footer from "./components/footer.svelte";
     import Navbar from "./components/navbar.svelte";
     import { Section, Quotes, Testimonial, TestimonialCard, TestimonialCardItem } from 'flowbite-svelte-blocks';
     import Profile from "$lib/assets/profile.jpg";
     import { Marquee } from 'flowbite-svelte'
     import React from "$lib/assets/react.png";
    import Angular from "$lib/assets/angular.png";
    import Vue from  "$lib/assets/vue.png";
    import Sveltekit from  "$lib/assets/svelte.png";
    
  
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

<main style="display: flex; flex-direction: column; justify-content: center; align-items: center; height: 100vh;">
    <div class="flex justify-center flex-row justify-center items-center content-center max-w-screen-md flex-col m-auto text-center">
        <div class="m-auto p-5">
            <p class="md:text-6xl text-4xl font-black dark:text-slate-100 pt-2 tracking-tight text-gray-950">LEAN RESOURCES</p>
            <p class="md:text-lg text-xs pt-5 text-orange-400 tracking-tight">Your Easy Path to Coding Resources💻</p>
            <a href="/all-pages"><button class="bg-orange-500 p-2 pl-5 pr-5 hover:scale-[1.2] cursor-pointer text-white mt-6 rounded-lg font-semibold border border-orange-400 hover:border-slate-400">Explore Now🚀</button></a>
        </div>
    </div>
    <Marquee speed={0.5}  shadow class="py-5">
        <img class="w-16 h-16" alt="flowbite-svelte icon logo" src={React} />
        <img class="w-16 h-16" alt="flowbite-svelte icon logo" src={Vue} />
        <img class="w-16 h-16" alt="flowbite-svelte icon logo" src={Angular}/>
        <img class="w-16 h-16" alt="flowbite-svelte icon logo" src={Sveltekit} />
    </Marquee>
</main>
<div style="height: 60vh; margin-top: 20rem;">
    <Section name="testimonial">
        <Testimonial icon={Quotes}>
          <blockquote>
            <p class="text-lg lg:text-xl font-medium text-gray-900 dark:text-white">"All the resources you need, neatly listed for you. Tutorials, tools, and more - discover it all effortlessly.👌🏼"</p>
          </blockquote>
          <svelte:fragment slot="footer">
            <img class="w-6 h-6 rounded-full" src={Profile} alt="michael profile" />
            <div class="flex items-center divide-x-2 divide-gray-500 dark:divide-gray-700">
              <div class="pr-3 font-medium text-gray-900 dark:text-white">Jan Leander</div>
              <div class="pl-3 text-sm font-light text-gray-500 dark:text-gray-400">Creator of Lean Resources</div>
            </div>
          </svelte:fragment>
        </Testimonial>
      </Section>
</div>


<div class="pt-10 pb-20">
    <Footer></Footer>
</div>

 <style lang="postcss">
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
 
