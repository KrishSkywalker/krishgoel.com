<script>
    let title= "Projects | krishgoel.com";
    let description = "A detailed index of all the projects I have worked on so far. Hi, I'm Krish! A technophile and an engineering student from New Delhi.";
    let url = "https://krishgoel.com/projects";

    let arrayOfTwo = [0,1];
    let arrayOfFour = [0, 1, 2, 3];
    let projectCards = [
		{
            imageID: "gyaan-academy",
            title: "The Gyaan Academy", 
            date: "September 2020",
            type: "🚀 Concept Documentation",
            pretext: "Amartya, Kataria and I built this startup idea ground up in 72 hours for an interschool IT event. The idea is an 'Online School' with smart features including building a network.",
            tags: {
                tag1: "E-ducation",
                tag2: "Life skills",
                tag3: "Future"
            },
            linkText: "📁 Documentation",
            url: "https://krishgoel.herokuapp.com/projects/gyaanacademy"
        },
        {
            imageID: "vkyd",
            title: "VKYD", 
            date: "July 2020",
            type: "⚙️ Work in progress",
            pretext: "VKYD is a upcoming smart streetwear fashion platform. I aim to evolve it into a social commerce platform.",
            tags: {
                tag1: "Sustainable fashion",
                tag2: "Streetwear",
                tag3: "Social commerce"
            },
            linkText: "🌐 Website",
            url: "http://vkyd.in"
        },
        {
            imageID: "eyena",
            title: "Eyena", 
            date: "May 2020",
            type: "🚀 Concept Documentation",
            pretext: "Eyena is an IoT based smart mirror that measures your body temperature upon detecting your presence without any physical contact. The project isn't econonmically feasible with the current technology, hence I had to postpone it indefinitely.",
            tags: {
                tag1: "Thermal imaging",
                tag2: "COVID-19",
                tag3: "Hardware dev"
            },
            linkText: "📁 Documentation",
            url: "http://eyena.krishgoel.com"
        },
        {
            imageID: "",
            title: "Portfolio Page",
            date: "September 2019",
            type: "👍 (Never) Completed",
            pretext: "I wanted a platform to showcase all that I have done and will be doing while relfecting my personal taste in design and being dynamic enough for easy and quick updation, hence this webpage.",
            tags: {
                tag1: "Portfolio",
                tag2: "Svelte",
                tag3: "Vercel"
            },
            linkText: "💻 Github Repository",
            url: "https://github.com/KrishSkywalker/krishgoel.com"
        },
        {
            imageID: "lunatix",
            title: "Lunatix", 
            date: "October 2019",
            type: "🚀 Concept Documentation",
            pretext: "A project that Raghav Sarangi, Kartik Gupta and I worked on for an IT event - Exun 2019. This was an idea documentation that aimed at agricultural development on the lunar surface.",
            tags: {
                tag1: "Lunar Agriculture",
                tag2: "Space Tech",
                tag3: "Idea pitch"
            },
            linkText: "📁 Documentation",
            url: "https://drive.google.com/drive/folders/1E7EJTsJhww2c5vz1DRLYnc9JRg6RynOU"
        },
        {
            imageID: "binary-box",
            title: "Binary Box",
            date: "September 2019",
            type: "🚀 Concept Documentation",
            pretext: "A subscription-based STEM Kits delivery service model that Kartik Gupta and I developed for an IT event.",
            tags: {
                tag1: "STEM",
                tag2: "Startup Idea",
                tag3: "Subscription Model"
            },
            linkText: "📁 Documentation",
            url: "/projects/binarybox"
        },
        {
            imageID: "alexation",
            title: "Alexation",
            date: "June 2019",
            type: "👍 Completed",
            pretext: "Not very original, but this project eliminated the need of a central Alexa hub by creating an ecosystem using NodeMCU. It brings down the cost of automation from $20 to $3 per device.",
            tags: {
                tag1: "NodeMCU",
                tag2: "IoT",
                tag3: "Home Automation"
            },
            linkText: "💻 Github Repository",
            url: "https://github.com/KrishSkywalker/alexation"
        },
        {
            imageID: "",
            title: "teayamo.com",
            date: "September 2017",
            type: "👍 Completed",
            pretext: "This was my first 'large-scale' web project with loads of pages that I made without tempplating 😞😜. It was for my dad's tea startup and gave me a solid introduction to big-scale webdev.",
            tags: {
                tag1: "Tea Startup",
                tag2: "Large scale dev",
                tag3: ""
            },
            linkText: "🌐 Website",
            url: "http://www.teayamo.com"
        },
        {
            imageID: "",
            title: "Arduino Drumpads",
            date: "August 2017",
            type: "👍 Completed",
            pretext: "I designed e-drums while eliminating the MIDI and laptop requirements that require close to none setup and make it more cost-effective",
            tags: {
                tag1: "Arduino",
                tag2: "MIDI",
                tag3: "EDM"
            },
            linkText: "💻 Github Repository",
            url: "https://github.com/KrishSkywalker/arduino-drum-pads"
        },
        {
            imageID: "",
            title: "Anet A8 3D Printer",
            date: "December 2016",
            type: "👍 Completed",
            pretext: "I designed and assembled this Anet A8 inspired 3D printer with a 0.5mm X-Y-Z slicing precision and 22cm cube printing volume.",
            tags: {
                tag1: "3D Printing",
                tag2: "Hardware",
                tag3: ""
            },
            linkText: "",
            url: ""
        }
	];
</script>

<style>
    .projects .card {
        padding-top: 0px;
    }
    .projects .card img{
        border-bottom-left-radius: 0;
        border-bottom-right-radius: 0;
    }
</style>

<svelte:head>
    <title>{title}</title>
    <meta name="title" content="{title}" />
    <meta name="description" content="{description}" />
    <meta property="og:title" content="{title}" />
    <meta property="og:url" content="{url}" />
    <meta property="og:description" content="{description}" />
    <meta name="twitter:title" content="{title}" />
    <meta name="twitter:url" content="{url}" />
    <meta name="twitter:description" content="{description}" />
</svelte:head>

<section class="projects">
    <h1 class="mono">All of my projects</h1>
    <p>🌐 A detailed index of all the projects I have worked on so far</p>
    
	<!-- Mobile Screen Layout -->
	<div class="small-screen">
		{#each projectCards as project, index}
		<div class="card">
            {#if project.imageID != ""}
                <img src="images/projects/{project.imageID}.png">
            {:else}
                <br>
            {/if}
			<div class="width-restriction">
				<h2>{project.title}</h2>
				<h5 class="mono">{project.date}</h5>
				<h6>{project.type}</h6>
				<p>{project.pretext}</p>
				<div class="tags">
                    {#if project.tags.tag1 != ""}
                        <div class="tag">
                            <p>{project.tags.tag1}</p>
                        </div>
                    {/if}
					{#if project.tags.tag2 != ""}
                        <div class="tag">
                            <p>{project.tags.tag2}</p>
                        </div>
                    {/if}
                    {#if project.tags.tag3 != ""}
                        <div class="tag">
                            <p>{project.tags.tag3}</p>
                        </div>
                    {/if}
				</div>
                {#if project.linkText != ""}
                    <br>
                    <br>
                    <a href={project.url}>{project.linkText}</a>
                {/if}
			</div>
		</div>
		{/each}
    </div>
    
	<!-- Mid Screen Layout -->
	<div class="mid-screen">
        <div class="col-container">
            {#each arrayOfTwo as i, index}
                <div class="col-2">
                    {#each projectCards as project, index}
                        {#if index%2 == i}
                            <div class="card">                            
                                {#if project.imageID != ""}
                                    <img src="images/projects/{project.imageID}.png">
                                {:else}
                                    <br>
                                {/if}
                                <div class="width-restriction">
                                    <h2>{project.title}</h2>
                                    <h5 class="mono">{project.date}</h5>
                                    <h6>{project.type}</h6>
                                    <p>{project.pretext}</p>
                                    <div class="tags">
                                        {#if project.tags.tag1 != ""}
                                            <div class="tag">
                                                <p>{project.tags.tag1}</p>
                                            </div>
                                        {/if}
                                        {#if project.tags.tag2 != ""}
                                            <div class="tag">
                                                <p>{project.tags.tag2}</p>
                                            </div>
                                        {/if}
                                        {#if project.tags.tag3 != ""}
                                            <div class="tag">
                                                <p>{project.tags.tag3}</p>
                                            </div>
                                        {/if}
                                    </div>
                                    {#if project.linkText != ""}
                                        <br>
                                        <br>
                                        <a href={project.url}>{project.linkText}</a>
                                    {/if}
                                </div>
                            </div>
                        {/if}
                    {/each}
                </div>
            {/each}
        </div>
    </div>

    <!-- Large Screen Layout -->
    <div class="large-screen">
        <div class="col-container">
            {#each arrayOfFour as i, index}
                <div class="col-4">
                    {#each projectCards as project, index}
                        {#if index%4 == i}
                            <div class="card">                            
                                {#if project.imageID != ""}
                                    <img src="images/projects/{project.imageID}.png">
                                {:else}
                                    <br>
                                {/if}
                                <div class="width-restriction">
                                    <h2>{project.title}</h2>
                                    <h5 class="mono">{project.date}</h5>
                                    <h6>{project.type}</h6>
                                    <p>{project.pretext}</p>
                                    <div class="tags">
                                        {#if project.tags.tag1 != ""}
                                            <div class="tag">
                                                <p>{project.tags.tag1}</p>
                                            </div>
                                        {/if}
                                        {#if project.tags.tag2 != ""}
                                            <div class="tag">
                                                <p>{project.tags.tag2}</p>
                                            </div>
                                        {/if}
                                        {#if project.tags.tag3 != ""}
                                            <div class="tag">
                                                <p>{project.tags.tag3}</p>
                                            </div>
                                        {/if}
                                    </div>
                                    {#if project.linkText != ""}
                                        <br>
                                        <br>
                                        <a href={project.url}>{project.linkText}</a>
                                    {/if}
                                </div>
                            </div>
                        {/if}
                    {/each}
                </div>
            {/each}
        </div>
    </div>
</section>