<script>
    let arrayOfTwo = [0, 1];
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

<section class="blog-section">
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
    <p>
        You may find the rest of articles @ 
        <a href="/blog" aria-label="The Blog" class="mono">/blog</a>
    </p>
</section>