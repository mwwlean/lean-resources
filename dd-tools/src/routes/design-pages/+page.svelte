<script>
    import { Card } from 'flowbite-svelte';
    import { Footer, FooterCopyright, FooterLinkGroup, FooterBrand, FooterLink } from 'flowbite-svelte';
    import { Popover, Button, Avatar } from 'flowbite-svelte';
    import Profile from "$lib/assets/profile.jpg";
    import Figma from "$lib/assets/figma.png";
    import Xd from  "$lib/assets/adobe-xd.png";
    import Photoshop from  "$lib/assets/photoshop.png";
    import Canva from  "$lib/assets/canva.png";
 </script>
 
 <div class="flex justify-center mt-16 text-4xl dark:text-slate-50 font-semibold">Design Tools 🎨</div>
 <div class="max-w-screen-lg m-auto grid md:grid-cols-3 gap-6 mt-16 justify-center">  
        <Card href="/cards" class="col-span-1" >
            <img src={Figma} alt="Figma" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Figma</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Figma is a collaborative design tool in the cloud, allowing users to create, prototype, and iterate on interface designs seamlessly.</p>
        </Card>
        
        <Card href="/cards" class="col-span-1" >
            <img src={Xd} alt="Adobe XD" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Adobe XD</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Adobe XD is Adobe's design and prototyping tool for creating user experiences in web and mobile applications.</p>
        </Card>
        
        <Card href="https://www.adobe.com/products/photoshop.html" class="col-span-1" >
            <img src={Photoshop} alt="Adobe Photoshop" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Adobe Photoshop</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
                Adobe Photoshop is a versatile raster graphics editing software used for tasks like photo editing, graphic design, and digital art creation.</p>
        </Card>
        <Card href="/cards" class="col-span-1" >
            <img src={Canva} alt="Canva" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Canva</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight text-sm">Canva is a user-friendly online graphic design platform for creating a variety of visual content, from social media graphics to presentations.</p>
        </Card>
        
        <Card href="/cards" class="col-span-1" >
            <img src="https://cdn.sanity.io/images/wd3e2pma/production/7b336dc26fd85ae98b414761d58238d225876a88-60x48.svg" alt="Zeplin" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Zeplin</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">Zeplin is a design collaboration and handoff tool that streamlines communication between designers and developers by providing a platform for sharing and implementing design specifications.</p>
        </Card>
        
        <Card href="https://www.adobe.com/products/photoshop.html" class="col-span-1" >
            <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAHcAAAB3CAMAAAAO5y+4AAAAllBMVEXwhwXfbAz////dYQDwxK/fagDhbwvwhQD97ePwgwDwhxD+8+r//vzifkbxlEjxjijgcSHkhkvvfAD2uofvvaTki1voegndXQD34NTrfwfkdAr75NP3w5niezz89O/118jnmW/tsZL1rnT0qmrxlDz5zav51r7ym0/2vZHxo2nhdjTxjjbpoHvjg1DcVQD1s3zrqIfmlGU7M8bdAAADoUlEQVRoge3b2VriMBQA4JAQQ6AOEpZ2rJYWFRUZxfd/ubFDygfN3iZ0LnouwfTnZOtJEQBhupkScL0g400KIYAPjF6T/YEpe4AgZVdFj8FS8EQ7cOkGjDtgAZl2oZZwR24fffwfQeQRGGV0LA/KAu579PklHSli+xoMpm9QFy+B7mv0QcuWcAiW/DKwEL6HgNnW6Cb3/lkyHhndbPfbvzudGN3oFnuHLd2Bb9jW9Q1bu55he9cv7OB6hV1cn7CT6xF2c/3Bju5NR6432NX1BTu7nmB31w/cwPUCN3F9wI1cD3Aztz1sU+dEj4LbHqap0U1EdjBoW+vRJ6N7QBK3PWwqZKXptocJ0Pd0cqdwW8Nsrp7TkwKpWA9d/cGV/bKKnL/yRzq2nmDG19L6E1cRD48vZZ86tx1Mv3hyZyOJB9HxtUKbcBuYUE4szgl04B9moB7fMlbN033hU+gSQLzzt/qEG8P0mSeWXwL4u5pa+oSbwtW+sa7nFfM3EkPCzWC6OV49EtLCu+z4lnyfbAef7kdD8eKo4GtJuWNV4V5WszfdtavPFBtcZ5h8RJq+RNXUmpkSdoWZfu6gNX/bmLAbfLr5KhLCu2rjNk0tN5ipJxVPeMGH39jRLjCdG/fCmK+lhbmnrWEyNu/9eM+X985fxoxvzJkulzjh25lFwnYwOW3MulTwjP/V0iJhq+qWpVaLpKoAJhYJ27jVGpJV5RcJW1YAli6htjPVtgJQuYSeB+OPuzOEsHZ8Maqm1jBG5yFpJXEJe/2an8Ub773t/rC/jVUyjh/3hwMfYThcnEWRi7Lo0tcRhyQRrRWrE+/W6lYw+66PuODSd3Xzf5cQj5ol+2g4pNbvYnX3tFSVMZJOmsTUbKZ/AmHxJYLkBlztkZqoFWU11+ZQL7kDx8Z0YXY5Mequ+buan44W8zU/CoDaR0w27kQssGzcWet8e7d3e7d3e7d3e7cDt856cIPVV5G2vrKpJyWnLtS2nrSon2XPr/DA2NG1Q7F4Xpjr20fSUzWeaU4pZdQ7SXI+es807RPpMaU8qOiGOBOeLknOg3SVL4byKJbK7y4wWhaKVov8TpwSogvACqlCe/5Vt5I0k7lgpbm8p5C6V4DlbnhY4QaHVW5oWOkGhtVuWFjjBoV1bkhY6waE9W442OAGg01uKNjogvuO3DCwzS9FQsBg3Al8AzY2/6PtG8a55e+tPMNxYvv7Mp8wjgsIyt/TXXeMb/Kfmvcv2Jhhu6NnRC4AAAAASUVORK5CYII=" alt="Draw IO" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Draw IO</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
               Draw IO is a web-based tool for creating diagrams, flowcharts, and visual representations. It's widely used for its user-friendly interface and collaborative features.</p>
        </Card>
        <Card href="https://www.adobe.com/products/photoshop.html" class="col-span-1" >
            <img src="https://th.bing.com/th?id=ODLS.804f77d1-b30b-4608-b167-d735609e91fe&w=32&h=32&qlt=90&pcl=fffffa&o=6&pid=1.2" alt="Framer" class="w-14 h-14">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white pt-2">Framer</h5>
            <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight  text-sm">
                Framer is a design and prototyping tool that empowers designers to create interactive user interfaces with a focus on dynamic user experiences.</p>
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