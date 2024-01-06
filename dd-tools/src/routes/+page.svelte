<script>
     import Footer from "./components/footer.svelte";
     import Navbar from "./components/navbar.svelte";
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
<div class="back_to_start" on:click={goStart} class:hidden>Back To Start</div>
<main style="display: flex; flex-direction: column; justify-content: center; align-items: center; height: 90vh;">
    <div class="flex justify-center flex-row justify-center items-center content-center max-w-screen-md flex-col m-auto text-center">
        <div class="m-auto p-5">
            <p class="md:text-lg text-xs pt-5 text-orange-400 tracking-tight">Your Easy Path to Coding Resources💻</p>
            <p class="md:text-6xl text-4xl font-black dark:text-slate-100 pt-2 tracking-tight text-gray-950">LEAN RESOURCES</p>
            <p class="md:text-lg text-base font-light pt-3 dark:text-slate-100 text-gray-700">All the resources you need, neatly listed for you. Tutorials, tools, and more - discover it all effortlessly.👌🏼</p>
            <a href="/all-pages"><button class="bg-orange-500 p-2 pl-5 pr-5 hover:scale-[1.2] cursor-pointer text-white mt-6 rounded-lg font-semibold border border-orange-400 hover:border-slate-400">Get started 🚀</button></a>
        </div>
    </div>
</main>



<Footer></Footer>


 <style lang="postcss">
   .back_to_start {
        opacity: 1;
        transition: opacity 0.5s, visibility 0.5s;
        position: fixed;
        z-index: 99;
        right: 20px;
        user-select: none;
        bottom: 20px;
        color: yellow;
        background-color: black;
        padding: 5px;
        font-weight: 700;
        border-radius: 5px;
    }

    .back_to_start.hidden {
        opacity: 0;
        visibility: hidden;
    }
 </style>
 
