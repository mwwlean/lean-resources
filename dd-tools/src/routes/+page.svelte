<script>
     import Footer from "./components/footer.svelte";
     import Sidebar from "./components/Sidebar.svelte";
     import Main from "./components/Main.svelte";
     import Hero from "./components/hero.svelte";

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


<Main></Main>

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
 
