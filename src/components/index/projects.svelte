<style>
    @media screen and (max-width: 600px) {
        .large-screen, .mid-screen {
            display: none
        }
    }
    @media screen and (min-width: 600px) and (max-width: 800px) {
        .small-screen, .large-screen {
            display: none
        }
    }
    @media screen and (min-width: 800px) {
        .small-screen, .mid-screen {
            display: none
        }
    }

    .card {
        padding: 0px;
        padding-bottom: 30px;
    }

    .card img {
        width: 100%;
        padding-bottom: 20px
    }

    .card h6 {
        font-weight: 400
    }

    :global(body.dark-mode) .card {
        background-color: #000000;
        box-shadow: rgba(36, 36, 36, 0.89) 7px 7px 21px -10px;
    }
    :global(body.dark-mode) .card .tags .tag {
        background-color: #ffffff00;
        border: 2px solid #ffffff
    }
    :global(body.dark-mode) .card p a {
        color: #ffffff
    }
    :global(body.dark-mode) .card a {
        color: #ffffff
    }
</style>

<script>
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
            url: ""
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
            url: ""
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
            url: ""
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
            url: ""
        }
	];
</script>

<div class="width-restriction">
    <h1 class="mono">🌐 Featured Projects</h1>
    
	<!-- Mobile Screen Layout -->
	<div class="small-screen">
		{#each projectCards as project, index}
		<div class="card">
			<img src="images/projects/{project.imageID}.png">
			<div class="width-restriction">
				<h2>{project.title}</h2>
				<h5 class="mono">{project.date}</h5>
				<h6>{project.type}</h6>
				<p>{project.pretext}</p>
				<div class="tags">
					<div class="tag">
						<p>{project.tags.tag1}</p>
					</div>
					<div class="tag">
						<p>{project.tags.tag2}</p>
					</div>
					<div class="tag">
						<p>{project.tags.tag3}</p>
					</div>
				</div>
				<br>
				<br>
				<a class="bold" href={project.url}>{project.linkText}</a>
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
                                <img src="images/projects/{project.imageID}.png">
                                <div class="width-restriction">
                                    <h2>{project.title}</h2>
                                    <h5 class="mono">{project.date}</h5>
                                    <h6>{project.type}</h6>
                                    <p>{project.pretext}</p>
                                    <div class="tags">
                                        <div class="tag">
                                            <p>{project.tags.tag1}</p>
                                        </div>
                                        <div class="tag">
                                            <p>{project.tags.tag2}</p>
                                        </div>
                                        <div class="tag">
                                            <p>{project.tags.tag3}</p>
                                        </div>
                                    </div>
                                    <br>
                                    <br>
                                    <a class="bold" href={project.url}>{project.linkText}</a>
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
                                <img src="images/projects/{project.imageID}.png">
                                <div class="width-restriction">
                                    <h2>{project.title}</h2>
                                    <h5 class="mono">{project.date}</h5>
                                    <h6>{project.type}</h6>
                                    <p>{project.pretext}</p>
                                    <div class="tags">
                                        <div class="tag">
                                            <p>{project.tags.tag1}</p>
                                        </div>
                                        <div class="tag">
                                            <p>{project.tags.tag2}</p>
                                        </div>
                                        <div class="tag">
                                            <p>{project.tags.tag3}</p>
                                        </div>
                                    </div>
                                    <br>
                                    <br>
                                    <a class="bold" href={project.url}>{project.linkText}</a>
                                </div>
                            </div>
                        {/if}
                    {/each}
                </div>
            {/each}
        </div>
    </div>
    <br>
    <br>
    <p>
        Check out all of my projects <a>here</a>
    </p>
</div>