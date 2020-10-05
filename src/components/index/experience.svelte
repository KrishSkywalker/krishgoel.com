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

    .card .progress-bar-container {
        width: 100%;
        border-radius: 10px;
        height: 15px;
        background-color: #969595;
    }

    .card .progress-bar {
        position: relative;
        top: 0;
        border-radius: 10px;
        height: 15px;
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
    let experienceCards = [
		{
            title: "1 The Gyaan Academy", 
            subhead: "Dub so big",
            pretext: "Amartya, Kataria and I built this startup idea ground up in 72 hours for an interschool IT event. The idea is an 'Online School' with smart features including building a network.",
            linkText: "📁 Documentation",
            url: ""
        },
        {
            title: "1 The Gyaan Academy", 
            subhead: "Dub so big",
            pretext: "Amartya, Kataria and I built this startup idea ground up in 72 hours for an interschool IT event. The idea is an 'Online School' with smart features including building a network.",
            linkText: "📁 Documentation",
            url: ""
        },
        {
            title: "1 The Gyaan Academy", 
            subhead: "Dub so big",
            pretext: "Amartya, Kataria and I built this startup idea ground up in 72 hours for an interschool IT event. The idea is an 'Online School' with smart features including building a network.",
            linkText: "📁 Documentation",
            url: ""
        },
        {
            title: "1 The Gyaan Academy", 
            subhead: "Dub so big",
            pretext: "Amartya, Kataria and I built this startup idea ground up in 72 hours for an interschool IT event. The idea is an 'Online School' with smart features including building a network.",
            linkText: "📁 Documentation",
            url: ""
        },
        {
            title: "1 The Gyaan Academy", 
            subhead: "Dub so big",
            pretext: "Amartya, Kataria and I built this startup idea ground up in 72 hours for an interschool IT event. The idea is an 'Online School' with smart features including building a network.",
            linkText: "📁 Documentation",
            url: ""
        },
        {
            title: "1 The Gyaan Academy", 
            subhead: "Dub so big",
            pretext: "Amartya, Kataria and I built this startup idea ground up in 72 hours for an interschool IT event. The idea is an 'Online School' with smart features including building a network.",
            linkText: "📁 Documentation",
            url: ""
        }
	];
</script>

<div class="width-restriction">
    <h1 class="mono">🎯 Experience</h1>
    
	<!-- Mobile Screen Layout -->
	<div class="small-screen">
        {#each experienceCards as experience, index}
            <div class="card">
                <div class="width-restriction">
                    <h2>{experience.title}</h2>
                    <h6>{experience.subhead}</h6>
                    <p>{experience.pretext}</p>
                    <a href={experience.url}>🔗 {experience.linkText}</a>
                </div>
            </div>
        {/each}
    </div>

    <!-- Mid Screen Layout -->
    <div class="mid-screen">
        <div class="col-container">
            {#each arrayOfTwo as i, index}
                <div class="col-2">
                    {#each experienceCards as experience, index}
                        {#if index%2 == i}
                            <div class="card">
                                <div class="width-restriction">
                                    <h2>{experience.title}</h2>
                                    <h6>{experience.subhead}</h6>
                                    <p>{experience.pretext}</p>
                                    <a href={experience.url}>🔗 {experience.linkText}</a>
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
                    {#each experienceCards as experience, index}
                        {#if index%4 == i}
                            <div class="card">
                                <div class="width-restriction">
                                    <h2>{experience.title}</h2>
                                    <h6>{experience.subhead}</h6>
                                    <p>{experience.pretext}</p>
                                    <a href={experience.url}>🔗 {experience.linkText}</a>
                                </div>
                            </div>
                        {/if}
                    {/each}
                </div>
            {/each}
        </div>
    </div>

</div>