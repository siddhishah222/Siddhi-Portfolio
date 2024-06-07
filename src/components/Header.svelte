<script>
    import { onMount } from 'svelte';

    let showPhoneNumber = false;

    function togglePhoneNumber() {
        showPhoneNumber = !showPhoneNumber;
    }

    export let y;
    export let tabs = [
        { name: "Projects", link: "#projects"},
        { name: "About me", link: "#about"},
        { name: "Recommendations", link: "#recommendations"},
        { name: "Contact", link: "#contact"},
    ];
</script>

<header
    class={"sticky z-[10] top-0 duration-200 px-6 flex items-center justify-between border-b border-solid " +
        ( y > 0
            ? " py-4 bg-slate-950 border-violet-950"
            : " py-6 bg-transparent border-transparent"
        )}
    >
    <h1 class="font-medium">
        <b class="font-bold poppins">Siddhi Shah</b>
    </h1>
    <div
        class="flex items-center gap-4 sm:gap-6 text-2xl sm:text-3xl md:text-4xl mx-auto mr-60"
    >
        <a 
            href="https://www.linkedin.com/in/siddhi-shah-developer/" 
            target="_blank" 
            class=""
        >
            <i class="fa-brands fa-linkedin-in text-3xl"/>
        </a>
        <a 
            href="https://github.com/siddhishah222" 
            target="_blank" 
        >
            <i class="fa-brands fa-github text-3xl" />
        </a>
    </div>
    <div class="sm:flex items-center gap-4 hidden">
        {#each tabs as tab, index}
            <a
                href={tab.link}
                class="duration-200 hover:text-violet-400"
            >
                <p>{tab.name}</p>
            </a>
        {/each}
 
        <button 
            on:click={togglePhoneNumber}
            class="blueShadow relative overflow-hidden px-5 py-2 group rounded-full bg-white text-slate-950">
            <div
                class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
            />
            <h4 id="contact" class="relative z-9">Let's chat</h4>
        </button>
        {#if showPhoneNumber}
            <p class="text-violet-400">Phone: +1(437) 985-7830</p>
        {/if}
    </div>
</header>