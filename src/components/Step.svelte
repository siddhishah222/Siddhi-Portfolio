<script>
    export let step;
</script>

<div
    class="p-4 sm:p-6 md:p-8 flex flex-col gap-4 rounded-lg border border-solid border-violet-700 text-center cursor-pointer group hover:border-violet-400 duration-200"
>
    <div
        class="bg-slate-950 grid place-items-center px-4 text-5xl md:text-6xl -mt-10 sm:-mt-12 md:-mt-14 lg:-mt-16 mx-auto duration-200"
    >
        <i class={step.icon} />
    </div>
    <h3 class="font-medium text-xl sm:text-2xl md:text-3xl">
        {step.name}
    </h3>
    <slot />
    <div class="flex-1 flex justify-between gap-4 items-end">
        {#if step.link}
            <div
                class="mr-auto mt-10 cursor-pointer duration-200 relative overflow-hidden"
            >
                <a 
                    href={step.link}
                    target="_blank" 
                    class="text-white hover:text-violet-400 z-4"
                >
                    Go to Application &rarr;
                </a>
            </div>
        {/if}

        <div class="flex-1 flex justify-between gap-4 items-start">
            {#if step.link1}
                <div
                    class="ml-auto mt-10 cursor-pointer duration-200 relative overflow-hidden"
                >
                    <a 
                        href={step.link1}
                        target="_blank" 
                        class="text-white hover:text-violet-400 z-4"
                    >
                        Go to Web &rarr;
                    </a>
                </div>
            {/if}
        </div>
    </div>
</div>
    <!-- <div class="flex-1 flex justify-between gap-4 items-end">
        <div
            class="mr-auto mt-10 cursor-pointer hover:text-slate-950 duration-200 relative after:absolute after:top-0 after:h-0 after:right-full after:bg-white after:w-full after:h-full rounded-full after:duration-200 hover:after:translate-x-full after:z-[-1] overflow-hidden"
        >
            <a 
            href={step.link}
            target="_blank" 
            class="text-violet-400 z-4">Go to Application &rarr;</a>
        </div>
    </div>
    <div class="flex-1 flex justify-between gap-4 items-start">
        <div
            class="ml-auto cursor-pointer hover:text-slate-950 duration-200 relative after:absolute after:top-0 after:h-0 after:right-full after:bg-white after:w-full after:h-full rounded-full after:duration-200 hover:after:translate-x-full after:z-[-1] overflow-hidden"
        >
            <a 
            href={step.link1}
            target="_blank" 
            class="text-white-400 z-4">Go to Web &rarr;</a>
        </div>
    </div> -->
