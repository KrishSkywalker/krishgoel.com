<style>
    .card {
        padding: 30px 0px;
        width: 100%
    }
    .card .width-restriction {
        width: 90%
    }
    @media screen and (max-width: 750px) {
        .col-container {
            display: inline-block
        }
        .col-2 {
            display: block;
            width: 100%
        }
    }
    .card img {
        width: 100%;
        padding-bottom: 20px;
        border-radius: 10px
    }
    .card a, a {
        color: #3a4a4a;
        border-bottom: 1.5px solid #ffffff;
        transition: 0.2s;
        padding-bottom: 1px;
        font-size: 0.9rem
    }
    .card a:hover, a:hover {
        border-bottom-color: #3a3a3a;
    }

    :global(body.dark-mode) .card {
        background-color: #000000;
        box-shadow: rgba(36, 36, 36, 0.89) 7px 7px 21px -10px;
    }
    :global(body.dark-mode) .card p a {
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
    import Topnav from '../../components/common/topnav.svelte';
</script>

<svelte:head>
	<title>Gyaan Academy | krishgoel.com</title>
</svelte:head>

<Topnav />
<br><br><br><br><br><br>

<div class="width-restriction">
    <h1>Gyaan Academy</h1>
    <br>
    <h6>🚀 Idea documentation</h6>

    <!-- Introduction card -->
    <div class="card">
        <div class="width-restriction">
            <p> Hi there<br/>
                The Gyaan Academy was our (<a href="#">Amartya</a>, <a href="https://api.whatsapp.com/send?phone=919821943279&amp;amp;text=hLo%20Kattu%20bebsssssssss!&amp;amp;source=&amp;amp;data=&amp;amp;app_absent=">Kataria </a>and my) idea submission to the <a href="https://docs.google.com/document/d/1knMwl0VCeYnG0WUfCfavPYtO2b9VU1AvUCmYOuiRxLM/edit?usp=sharing">Make Prompt at MINET X 2020 </a>(more details to the competition can be found <a href="https://docs.google.com/document/d/1XGd4g70jAkGd0brlfFQCaIP5jXi_ntrQ6oKSC1wRlJI/edit?usp=sharing">here</a>) to solve not just 1 but all 17 Sustainable Development Goals for the 5 BRICS Nations. When we set out on our 60 hour journey to build this idea ground-up, our goal wasn't to win but to create, build something novel that could really be scaled to not just the 5 BRICS mentioned by the prompt but any region of the world, to make quality education more accessible.
                <br/><br/>
                Personally, I have always been passionate about changing the education system for good, teaching what's useful, what the student wants to learn and teaching to the point of perfection. While it is one of my life goals to build a school with the best in class infrastructure and state of the art curriculum, this competition gave me a chance to rethink all of that. Why do it then, why not now? Why only for the 3,000 kids who'll attend and not the millions who can do it online? Why only for the ones who'll be able to afford it? Why not everyone who deserves it? The Gyaan Academy answered all of that.
                <br/><br/>
                <span class="mono">
                    No flex but the event was judged by <a href="https://anandchowdhary.com/">Mr. Anand Chowdhary </a>(Creative technologist, Forbes 30 under 30).
                </span>
            </p>
        </div>
    </div>

    <!-- What is the Gyaan Academy? -->
    <div class="card">
        <div class="width-restriction">
            <h2>What is the Gyaan Academy?</h2>
            <div class="col-container">
                <div class="col-2">
                    <img src="images/gyaanacademy/deck/1.png">
                </div>
                <div class="col-2">
                    <img src="images/gyaanacademy/deck/2.png">
                </div>
            </div>
            <p>The Gyaan Academy isn't just another Udemy, it’s the new social network. While searching for solutions, we realised that every sustainable dev goal is a subset of the bigger problem - that lack of an educated population so, targeting this root cause would essentially mean eventually minimizing the others. Mahatama Gandhi described education as the mightiest means to shake the world, gently and that's where our thoughts coincided.</p>
        </div>
    </div>

    <!-- USPs -->
    <div class="card">
        <div class="width-restriction">
            <img src="images/gyaanacademy/deck/3.png">
            <h3>Learning what that matters more</h3>
            <p>The things we wanted to learn were never a part of the school syllabus or the content was inadequate, things like entrepreneurship, programming, culinary arts, financial education, even growing plants and hydroponics weren’t there and we believe they would have been much more helpful to us than the history lessons. Well, we don’t do that here, you’re taught only what you want to learn and to the point of perfection.<br/><br/>
            Being strong believers of Ikigai, we wanted our course selection algos and support to help you find yours.</p>
        </div>
    </div>
</div>