<style>
    @media screen and (max-width: 650px) {
        .large-screen {
            display: none
        }
    }
    @media screen and (min-width: 650px) {
        .small-screen {
            display: none
        }
    }

    .card a {
        border-bottom: 1.5px solid #ffffff;
        transition: 0.2s;
        padding-bottom: 5px;
        font-size: 0.9rem;
        font-weight: 400
    }
    .card a:hover {
        border-bottom-color: #3a3a3a;
    }

    :global(body.dark-mode) .card {
        background-color: #000000;
        box-shadow: rgba(36, 36, 36, 0.89) 7px 7px 21px -10px;
    }
    :global(body.dark-mode) .card .tags .tag {
        background-color: #ffffff00;
        border: 2px solid #ffffff
    }
    :global(body.dark-mode) .card p a{
        color: #ffffff
    }
    :global(body.dark-mode) .card a {
        color: #ffffff;
        border-bottom-color: #000000;
    }
    :global(body.dark-mode) .card a:hover {
        border-bottom-color: #ffffff;
    }
</style>

<script>
    let arrayOfTwo = [0, 1];
    // let products = JSON.parse(fs.readFileSync('data/products.json', 'utf8'));
    let blogCards = [
		{
            title: "My notes from 'The $100 Startup'", 
            status: "Coming soon",
            pretext: "Owing to my new-found passion in financial education and entrepreneurship, I am currently reading 'The $100 Startup' by Chris Guillebeau. This post includes my findings and notes from the book.",
            tags: {
                tag1: "Entrepreneurship",
                tag2: "Quick business deployment",
                tag3: "Scaling"
            },
            linkText: "🕓 Hold up m8",
            url: ""
        },
        {
            title: "Where I think I am headed", 
            status: "Coming soon",
            pretext: "I have always had different outlook of my future since my early childhood from being an astronaut and living inside a spaceshuttle to spend all of my dad's money and not do anything. This post talks about all of it and what I wanna do now.",
            tags: {
                tag1: "Business automation",
                tag2: "The 10-year goal",
                tag3: "Startup"
            },
            linkText: "🕓 Again, hol' up bro",
            url: ""
        }
	];
</script>

<div class="width-restriction">
    <h1 class="mono">📝 web.log(views)</h1>
    <!-- Mobile Screen Layout -->
    <div class="small-screen">
        {#each blogCards as card, index}
            <div class="card">
                <div class="width-restriction">
                    <h2>{card.title}</h2>
                    <h6>{card.status}</h6>
                    <p>{card.pretext}</p>
                    <div class="tags">
                        <div class="tag">
                            <p>{card.tags.tag1}</p>
                        </div>
                        <div class="tag">
                            <p>{card.tags.tag2}</p>
                        </div>
                        <div class="tag">
                            <p>{card.tags.tag3}</p>
                        </div>
                    </div>
                    <br><br>
                    <p>
                        <a href={card.url}>{card.linkText}</a>
                    </p>
                </div>
            </div>
        {/each}
    </div>

    <!-- Large Screen Layout -->
    <div class="large-screen">
        <div class="col-container">
            {#each arrayOfTwo as i, index}
                <div class="col-2">
                    {#each blogCards as card, index}
                        {#if (index+2)%2 == i}
                            <div class="card">
                                <div class="width-restriction">
                                    <h2>{card.title}</h2>
                                    <h6>{card.status}</h6>
                                    <p>{card.pretext}</p>
                                    <div class="tags">
                                        <div class="tag">
                                            <p>{card.tags.tag1}</p>
                                        </div>
                                        <div class="tag">
                                            <p>{card.tags.tag2}</p>
                                        </div>
                                        <div class="tag">
                                            <p>{card.tags.tag3}</p>
                                        </div>
                                    </div>
                                    <br><br>
                                    <p>
                                        <a href={card.url}>{card.linkText}</a>
                                    </p>
                                </div>
                            </div>
                        {/if}
                    {/each}
                </div>
            {/each}
        </div>
    </div>
</div>