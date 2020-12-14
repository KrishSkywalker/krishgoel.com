<style>
    .intro-section p a {
        padding-bottom: 5px;
        border-bottom: 1.5px solid rgba(0,0,0,0);
        transition: 0.2s;
    }
    .intro-section p a:hover {
        border-bottom: 1.5px solid var(--body)
    }

    @media screen and (max-width: 850px) {
        .small-screen {
            display: block;
        }
    }
    @media screen and (min-width: 851px) {
        .large-screen {
            display: block;
        }
    }
</style>

<section class="intro-section">
    <div class="large-screen">
        <div class="col-container">
            <div class="col-2">
                <div class="width-restriction">
                    <img src="/images/banner.png" alt="Krish Goel">
                </div>
            </div>
            <div class="col-2">
                <h1>Hi, I am Krish</h1>
                <h4 class="mono">or KrishSkywalker</h4>
                <br/>
                <p>
                    I’m a technophile and a full-time aspiring engineering student at <a href="https://sanskritischool.edu.in" class="svelte-1340r0r">Sanskriti School, New Delhi.</a>
                    <br>
                    <br>
                    Web development and programming being my métier, I’m currently learning how to teach the machines to think autonomously and working on a smart streetwear fashion startup.
                    <br>
                    <br>
                    Bricolage is my thing and I spent my last 2 summers teaching younger students the intricacies of coding. Looking at the bigger picture, I aspire to develop ‘smarter’ energy sources and solve global-ecological problems with the lines I type.
                    <br>
                    <br>
                    I recently found my passion in entrepreneurship and I&#39;m currently reading <a href="https://www.goodreads.com/book/show/12605157-the-100-startup" class="svelte-1340r0r">The $100 Startup by Chris Guillebeau</a>.
                </p>
            </div>
        </div>
    </div>

    <div class="small-screen">
        <img src="/images/banner.png" alt="Krish Goel">
        <h1>Hi, I am Krish</h1>
        <h4 class="mono">or KrishSkywalker</h4>
        <br/>
        <p>
            I’m a technophile and a full-time aspiring engineering student at <a href="https://sanskritischool.edu.in" class="svelte-1340r0r">Sanskriti School, New Delhi.</a>
            <br>
            <br>
            Web development and programming being my métier, I’m currently learning how to teach the machines to think autonomously and working on a smart streetwear fashion startup.
            <br>
            <br>
            Bricolage is my thing and I spent my last 2 summers teaching younger students the intricacies of coding. Looking at the bigger picture, I aspire to develop ‘smarter’ energy sources and solve global-ecological problems with the lines I type.
            <br>
            <br>
            I recently found my passion in entrepreneurship and I&#39;m currently reading <a href="https://www.goodreads.com/book/show/12605157-the-100-startup" class="svelte-1340r0r">The $100 Startup by Chris Guillebeau</a>.
        </p>
    </div>
</section>