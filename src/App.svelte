<script lang="ts">
    import "../node_modules/locomotive-scroll/dist/locomotive-scroll.css";
    import LocomotiveScroll from "locomotive-scroll";
    import { onMount } from "svelte";

    import americanFlag from "./assets/american_flag.png";
    import appealFlag from "./assets/appeal_to_heaven.png";
    import moultrieFlag from "./assets/fort_moultrie_flag.png";
    import sonsLibertyFlag from "./assets/sons_of_liberty_flag.png";

    onMount(() => {
        const scroll = new LocomotiveScroll({
            el: document.querySelector("[data-scroll-container]") as HTMLElement,
            smooth: true
        });

        return () => scroll.destroy();
    });
</script>

<div class="bg-zinc-900" data-scroll-container>
    <header class="min-h-svh flex flex-col justify-end p-8 relative">
        <span class="absolute top-4 right-8 text-4xl">
            &#127482&#127480
        </span>

        
        

        <h1 class="font-serif text-8xl text-zinc-50">Hello World</h1>
    </header>
    
    <main class="font-serif text-zinc-50 text-xl p-8 space-y-8 mb-16">
        <div class="grid grid-cols-4 gap-4 mb-8">
            <img data-scroll data-scroll-delay="0.1" data-scroll-speed="6" src={sonsLibertyFlag} alt="Sons of Liberty Flag" width="1920" height="1009" class="rounded" />
            <img data-scroll data-scroll-delay="0.3" data-scroll-speed="6" src={appealFlag} alt="American Flag" width="1920" height="1009" class="rounded translate-y-4" />
            <img data-scroll data-scroll-delay="0.5" data-scroll-speed="6" src={moultrieFlag} alt="Fort Moultrie Flag" width="1920" height="1377" class="rounded -translate-y-4" />
            <img data-scroll data-scroll-delay="0.7" data-scroll-speed="6" src={americanFlag} alt="American Flag" width="1920" height="1009" class="rounded translate-y-8" />
        </div>

        <div class="p-8 bg-red-500 rounded size-32 translate-x-full" data-scroll data-scroll-direction="horizontal" data-scroll-speed="36"></div>

        <p data-scroll data-scroll-delay="0.1" data-scroll-speed="6">Non vel tenetur et. Est quod et ea amet suscipit maxime. Iste animi ipsam pariatur. Et consectetur maxime voluptas aut harum. Voluptas a quia amet doloremque ut et nihil aliquid.</p>
        <p data-scroll data-scroll-delay="0.1" data-scroll-speed="6">Aliquam voluptatem nostrum odio consequatur excepturi reprehenderit. Optio totam voluptatum laboriosam molestiae non molestias consectetur corporis. Quisquam debitis ullam nesciunt incidunt facilis sit consequatur. Qui unde ea voluptas non quaerat similique natus. Doloremque minus pariatur eius voluptatum quis.</p>
        <p data-scroll data-scroll-delay="0.1" data-scroll-speed="6">Quam cumque impedit sed ipsa iure deserunt aperiam aut. Ratione nobis adipisci corporis itaque soluta aut velit. Excepturi qui voluptas corporis veritatis amet itaque. Labore et reiciendis dolorem architecto quo.</p>
        <p data-scroll data-scroll-delay="0.1" data-scroll-speed="6">Nihil aut hic quo eius recusandae tempore nesciunt quaerat. Deserunt voluptas in odio animi perspiciatis unde. Repudiandae velit occaecati eos tempora quia aut. Asperiores explicabo assumenda commodi repellendus ut magni. Tempora aliquam maiores soluta. Dolores modi ut et iusto reiciendis amet voluptate rerum.</p>
        <p data-scroll data-scroll-delay="0.1" data-scroll-speed="6">Sint vitae animi aperiam libero impedit. Non explicabo quia quasi sed alias ducimus. Eum reprehenderit libero odio.</p>

    </main>
    
    <footer class="text-xl p-8">
        <p>&#127482&#127480</p>
    </footer>
</div>
