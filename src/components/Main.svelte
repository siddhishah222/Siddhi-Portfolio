<script>
    import Step from "./Step.svelte";

    let steps = [
        {
            name: "CaaS (Communication as a Service)",
            icon: "fa-solid fa-envelope-open-text",
            description:
                "CaaS platform enables seamless communication across channels like email and Slack, enhancing collaboration and streamlining change management processes.",
        },
        {
            name: "Health Care",
            icon: "fa-solid fa-hospital-user",
            description:
                "Our Healthcare ecosystem includes web application for supervisors and admins, and mobile apps for clinicians on iOS and Android. It is created using React.js, Next.js, Storybook, Redux, Material UI, UI kittens and React Native. It connects Clinicians with career opportunities, and offers features such as competitive pay, the ability to manage work schedules, and access to a community for professional support and networking. ",
            // link: "https://play.google.com/store/apps/details?id=com.connectrn&hl=en_CA" ,
            // link1: "https://app.connectrn.com/"
        },
        {
            name: "DCLEX",
            icon: "fa-solid fa-coins",
            description:
                "DCLEX is a trading platform that enables users to settle trades in USDC and hold stocks in their Ethereum accounts.",
            link: "https://app.stg.dclex.com/stocks",
            link1: "https://dclex.com/?issueModal=0"
        },
        {
            name: "Global Settlement Service",
            icon: "fa-solid fa-globe",
            description:
                "Global Settlement Service is a platform designed to streamline and simplify the process of for new comers to settle in Canada. It includes web application and website for newcomers. It is created using React.js, Next.js, Storybook, Redux, WordPress and PHP.",
            link: "https://app.globalsettlementservice.com:3000/",
            link1: "https://globalsettlementservice.com/" ,
        },
        {
            name: "Tax Incentives Made Easy",
            icon: "fa-solid fa-money-bill-wave",
            description:
                "TIME Consulting is a platform that helps small and medium size businesses to secure funding from government to grow their business.",
            link1: "https://timeconsulting.ca/",
        },
        {
            name: "Cubic Digital",
            icon: "fa-solid fa-cube",
            description:
                "Cubic Digital provides comprehensive digital solutions tailored to meet the evolving needs of businesses in today's digital landscape.",
            link1: "https://cubicdigital.ca/"
        },
    ];

    let benefits = [
        {
            metric: "10x",
            name: "a self taught developer",
            description:
                "I am a self-taught developer who discovered a passion for coding through free online resources. The creativity and problem-solving involved in developing and engineering innovative online experiences captivated me. Beginning with JavaScript, HTML, and CSS, I have since expanded my expertise to include JavaScript frameworks, backend programming, design, cloud services, and much more.",
        },
        {
            name: "a product design & UX finatic",
            description:
                "Crafting and designing exceptional user experiences allows me to fully explore and express my creativity. I relish the challenge of learning new design concepts and empowering users through outstanding online interactions.",
        },
        {
            name: "an excellent communicator",
            description:
                "Communication is key and it's a paramount value of mine. I believe in transparency and constructive communication above all else. This helps me develop deep relationships and ensures my effectiveness and productivity in any work space with any team.",
        },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section 
        id="introPage" 
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
           class="flex flex-col lg:justify-center text-center lg:text-center gap-6 md:gap-8 lg:gap-10"
        >
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="poppins text-violet-400">Siddhi</span> Shah
                <br />Full Stack
                <span class="poppins text-violet-400">Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-violet-400"> favorite tech</span> 
                includes JavaScript, React.js, React Native, Next.js, SASS/SCSS, LESS, TailwindCSS, Node.js + express, PostgreSQL and Svelte. I specialize in building <span class="poppins text-violet-400"> responsive designs </span> with a keen focus on SEO, accessibility, and user experience.
            </p>
            <div class=" justify-center items-center">
                <a 
                    href="https://www.linkedin.com/in/siddhi-shah-developer/" 
                    target="_blank" 
                >
                    <button
                        class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
                    >
                        <div
                            class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                        />
                        <h4 class="relative z-9">
                            Let's connect &rarr;
                        </h4>
                    </button>
                </a>
            </div>
        </div>
        <div class="relative grid place-items-center">
            <div class="rounded-full p-0 m-4 bg-transparent shadow-5xl border-2 border-violet">
                <img
                    src={"images/Sidshahnew.png"}
                    alt="Siddhi Shah"
                    class="object-cover rounded-full max-h-[60vh]"
                />
            </div>
        </div>  
    </section>
    <section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                A few of my creative endeavors.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="poppins text-violet-400">see</span> my work?
            </h3>
        </div>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>
                Successfully launched the CaaS platform within the Nucleus ecosystem to streamline <strong class="text-violet-400"> Walmart's </strong> communication processes.  It is created using <strong
                class="text-violet-400"
                > React.js, Next.js, CSS preprocessors, Custom Hooks, React Hooks, Node.js, Express.js, and MongoDB.
                </strong> CaaS automated over <strong class="text-violet-400"> 200 </strong> Microsoft change event communications, <strong class="text-violet-400"> 150 </strong> Business Continuity and Disaster Recovery communications, saving <strong
                class="text-violet-400"
                > 460 man-hours </strong> annually.
                </p>
            </Step>
            <Step step={steps[1]}>
                <p>
                    Our Healthcare ecosystem includes application for supervisors, admins and clinicians on <strong
                    class="text-violet-400"
                    > web, iOS and Android. </strong> It is created using <strong
                    class="text-violet-400"
                    >React.js, Next.js, Storybook, Redux, React hooks, Material UI, UI kittens and React Native.</strong> It connects Clinicians with career opportunities, and offers features such as competitive pay, the ability to manage work schedules, and access to a community for professional support and networking.
                </p>
            </Step>
            <Step step={steps[2]}>
                <p>
                    DCLEX is a trading platform that enables users to settle trades in USDC and hold stocks in their Ethereum accounts. It is developed using <strong class="text-violet-400"
                        >React.js, TypeScript, Tailwind CSS, React Helmet, React Hooks, Redux, Web3 blockchain technology, Django and Docker.</strong
                    > Integrated real-time data feeds for comprehensive market insights, empowering users to make informed investment decisions swiftly.
                </p>
            </Step>
        </div>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[3]}>
                <p>
                    Global Settlement Service is a platform designed to streamline and simplify the process of for new comers to settle in Canada. It includes web application and website for newcomers. It is created using <strong class="text-violet-400"> React.js, Next.js, Storybook, Redux, React Hooks, Rest API, WordPress and PHP.</strong> I have created custom templated and themes for each web pages and content with <strong class="text-violet-400"> SEO</strong> in mind to ensure the platform ranks high on <strong class="text-violet-400">Google search index.</strong>
                </p>
            </Step>
            <Step step={steps[4]}>
                <p>
                    Tax Incentives Made Easy simplifies access to government funding for small and medium-sized businesses. The website utilizes a mix of <strong class="text-violet-400"> HTML, CSS, JavaScript, WordPress</strong> and backend technologies like <strong class="text-violet-400">PHP or Node.js</strong> for efficient processing. It may also leverage frameworks like <strong class="text-violet-400">React.js and Angular.js </strong> for interactive interfaces and WordPress for content management.
                </p>
            </Step>
            <Step step={steps[5]}>
                <p>
                    Cubic Digital specializes in comprehensive digital solutions, including SEO optimization. We leveraged strategies like keyword research, on-page optimization, technical SEO, content strategy, link building, and continuous monitoring to enhance online visibility and attract organic traffic. With used <strong class="text-violet-400">  HTML, CSS, JavaScript, WordPress, and PHP, </strong> to tailor solutions to meet the evolving needs of businesses in today's digital landscape.
                </p>
            </Step>
        </div>
    </section>
    <section
        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
        >
            <h6 class="text-large sm:text-xl md:text-2xl">
                Want to know more?
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="poppins text-violet-400">about</span> me.
            </h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
            I am . . .
        </p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <div class="flex gap-6 sm:gap-8">
                    <p
                        class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
                    >
                        0{index + 1}
                    </p>
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">
                            {benefit.name}
                        </h3>
                        <p>{benefit.description}</p>
                    </div>
                </div>
            {/each}
        </div>
        <h5 class={" text-2xl sm:text-3xl font-semibold text-center poppins "}>
            The <span class="text-violet-400">Complete</span> Package
        </h5>
        <div
            class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full"
        >
            <table class="bg-white text-slate-700 rounded text-center">
                <thead class={"border-b border-solid border-slate-200  "}>
                    <tr class="">
                        <th />
                        <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
                        <th
                            class="bg-violet-700 text-white whitespace-nowrap p-4 px-8"
                            >Me</th
                        >
                    </tr>
                </thead>
                <tbody>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Dedication</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Critical Thought</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr>
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Interpersonal Skills</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr class="border-t border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Progamming Ability</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                </tbody>
            </table>
        </div>
    </section>
    <section
        id="recommendations"
        class="py-20 pt-10 lg:pt-16 md:pb-0 flex flex-col gap-16 sm:gap-18 md:gap-20 relative"
    >
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
        >
            <h6 class="text-large sm:text-xl md:text-2xl">
                Here's how my coworkers describe our collaboration:
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                <span class="poppins text-violet-400">Recommendations</span>
            </h3>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/Anirvann.png"}
                alt="Partha's recommendation"
                class="object-cover z-[2] max-h-[32vh]"
            />
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/Rajendra.png"}
                alt="Rajendra's recommendation"
                class="object-cover z-[2] max-h-[40vh]"
            />
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/Gautam.png"}
                alt="Gautam's recommendation"
                class="object-cover z-[2] max-h-[83vh]"
            />
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/Amarjit.png"}
                alt="Amarjit's recommendation"
                class="object-cover z-[2] max-h-[40vh]"
            />
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/Partha.png"}
                alt="Partha's recommendation"
                class="object-cover z-[2] max-h-[49vh]"
            />
        </div>
        <p class="mx-auto mb-0 pb-0">So why not invest?</p> 
    </section>
</main>