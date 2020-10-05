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
    let repertoireCards = [
		{
            title: "1 The Gyaan Academy", 
            pretext: "Amartya, Kataria and I built this startup idea ground up in 72 hours for an interschool IT event. The idea is an 'Online School' with smart features including building a network.",
            completion: 20,
            linkText: "📁 Documentation",
            url: ""
        },
        {
            title: "2 The Gyaan Academy", 
            pretext: "Amartya, Kataria and I built this startup idea ground up in 72 hours for an interschool IT event. The idea is an 'Online School' with smart features including building a network.",
            completion: 78,
            linkText: "📁 Documentation",
            url: ""
        },
        {
            title: "3 The Gyaan Academy", 
            pretext: "Amartya, Kataria and I built this startup idea ground up in 72 hours for an interschool IT event. The idea is an 'Online School' with smart features including building a network.",
            completion: 78,
            linkText: "📁 Documentation",
            url: ""
        },
        {
            title: "4 The Gyaan Academy", 
            pretext: "Amartya, Kataria and I built this startup idea ground up in 72 hours for an interschool IT event. The idea is an 'Online School' with smart features including building a network.",
            completion: 78,
            linkText: "📁 Documentation",
            url: ""
        },
        {
            title: "5 The Gyaan Academy", 
            pretext: "Amartya, Kataria and I built this startup idea ground up in 72 hours for an interschool IT event. The idea is an 'Online School' with smart features including building a network.",
            completion: 78,
            linkText: "📁 Documentation",
            url: ""
        },
        {
            title: "6 The Gyaan Academy", 
            pretext: "Amartya, Kataria and I built this startup idea ground up in 72 hours for an interschool IT event. The idea is an 'Online School' with smart features including building a network.",
            completion: 78,
            linkText: "📁 Documentation",
            url: ""
        }
	];
</script>

<div class="width-restriction">
    <h1 class="mono">📄 My Repertoire</h1>
    
	<!-- Mobile Screen Layout -->
	<div class="small-screen">
        {#each repertoireCards as repertoire, index}
            <div class="card">
                <div class="width-restriction">
                    <h2>{repertoire.title}</h2>
                    <p>{repertoire.pretext}</p>
                    <div class="progress-bar-container">
                        <div class="progress-bar blue-green" style="width: {repertoire.completion}%"></div>
                    </div>
                </div>
            </div>
        {/each}
    </div>

    <!-- Mid Screen Layout -->
    <div class="mid-screen">
        <div class="col-container">
            {#each arrayOfTwo as i, index}
                <div class="col-2">
                    {#each repertoireCards as repertoire, index}
                        {#if index%2 == i}
                            <div class="card">
                                <div class="width-restriction">
                                    <h2>{repertoire.title}</h2>
                                    <p>{repertoire.pretext}</p>
                                    <div class="progress-bar-container">
                                        <div class="progress-bar blue-green" style="width: {repertoire.completion}%"></div>
                                    </div>
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
                    {#each repertoireCards as repertoire, index}
                        {#if index%4 == i}
                            <div class="card">
                                <div class="width-restriction">
                                    <h2>{repertoire.title}</h2>
                                    <p>{repertoire.pretext}</p>
                                    <div class="progress-bar-container">
                                        <div class="progress-bar blue-green" style="width: {repertoire.completion}%"></div>
                                    </div>
                                </div>
                            </div>
                        {/if}
                    {/each}
                </div>
            {/each}
        </div>
    </div>

</div>