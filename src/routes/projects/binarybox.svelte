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
    img {
        width: 100%;
        /* padding-bottom: 20px; */
        border-radius: 0px
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
import Projects from '../../components/index/projects.svelte';
</script>

<svelte:head>
	<title>Binary Box | krishgoel.com</title>
</svelte:head>

<Topnav />
<br><br><br><br><br><br>

<div class="width-restriction">
    <h1>Binary Box</h1>
    <br>
    <h6>🚀 Idea documentation</h6>

    <!-- Introduction card -->
    <div class="card">
        <div class="width-restriction">
            <h2>About</h2>
            <p>
                The BinaryBox was an MVP Startup idea that Kartik Gupta and I for 
                <a href="https://minet.co/">Make @ MINET X 2019</a>. We placed #3 at the Pitch event judged by creative technologists like <a href="https://anandchowdhary.com/">Anand Chowdhary</a>.
                <br/>BinaryBox is a subscription-based STEM Kits delivery service. We aim at developing a generation of imagineers who can change the world for the better with technology by their side. It provides hands-on knowledge and initial skills to get them interested in being future robotics engineers.
            </p>
            <br/>
            <h2>Problems that led us here</h2>
            <p>
                <li>The current STEM kits don’t give you the actual hands-on knowledge required to jump into the actual domain of STEM</li>
                <li>With the current STEM kits, you copy-paste what’s given in the manual. There is no actual understanding of the logic and workflow</li>
                <li>The STEM kits available don’t impart any life skills and limit your creativity to the box</li>
            </p>
            <br/>
            <h2>Our Story</h2>
            <p>
                We were fortunate enough to have recently visited the TERI facility in the village of Kathgodam in Uttarakhand. The minimal yet elaborate use of basic technology was something that touched us deeply. Impressed by this use of technology, we went on to create a solution to bring this joy to millions and here we are.
            </p>
            <br/>
            <h2>Company Ideology</h2>
            <p><span class="bold">Social mission: </span>On a mission to help produce an evolved generation that’s better adapted to STEM and work in tandem to make the world a better place because we believe in imagineers who can change the world for the better.</p>
            <p><span class="bold">Philanthropic philosophy: </span>The BB Privilege Programme The BinaryBox Privilege Programme is our philanthropic initiative wherein for every kit shipped, we take a percentage of our profits and use it to take tech-ed to remote areas.</p>
            <p><span class="bold">But why bother at all? </span>Technology is omnipresent and drives virtually everything in today’s world, with our kits, we create people who drive technology.</p>
            <p><span class="bold">Environmental initiative:</span> Minimalist design and care for nature (mostly in packaging)</p>
            <br/>
            <h2>Competitive advantage</h2>
            <p>It's <span class="bold">fun</span></p>
            <p>Gives you the <span class="bold">actual basic knowledge and initial skills </span>needed for entering the domain of programming and technological development</p>
            <p>Develops <span class="bold">logic and reasoning </span>that form the basis of programming and mathematics.</p>
            <p>Ensures that you <span class="bold">learn and not just copy-paste </span>using <span class="bold">encryption-decryption techniques, putting in order through workflow logics </span>and <span class="bold">explaining the logic </span>behind every line of code</p>
            <p>Not limited to just manuals, you can <span class="bold">add your creativity to the projects.</span></p>
            <p> <span class="bold">Imparts life skills</span>, you can even FAIL, the manual gives you the knowledge not the steps. After all, <span class="bold">“The greatest teacher, failure is” - Yoda</span></p>
            <p> We don’t give you a pre-programmed computer, you get the <span class="bold">actual microcontrollers </span>used by imagineers which are <span class="bold">programmed by you</span>. You don’t learn how to connect wires but how to <span class="bold">make things work</span></p>
            <p>You <span class="bold">learn the actual syntax</span> used by developers around the world</p>
            <p>Every monthly kit <span class="bold">comes with a theme and a relevant toy</span></p>
            <br/>
            <h2>The BB Privilege Programme</h2>
            <p>The BinaryBox Privilege Programme is our philanthropic initiative wherein for every kit shipped, we take a percentage of our profits and use it to take tech-ed to remote areas. <br/><br/>We aim at organising camps and workshops in remote regions of the world with the funds obtained. While we won’t be teaching topics as complex as microcontrollers for the beginning, we’ll be targeting to teach the basic use of computers and smartphones to increase the connectivity, not only for our prime audience - the kids but also the adults and grownups. We may as well promote volunteership and encourage our consumer base to help us teach at these workshops and lead by example.<br/><br/>Initially, in the budding stage, we’ll be looking at 30% - 40% of our profits being invested into the programme. However, as the company grows and breaks even, this percentage will rise to as high as 50%. </p>
            <br/>
            <h4>Promotion Strat and Exclusivity business model</h4>
            <p>Every kit comes with a unique code that once entered adds the kit to your account and enables the access to all the kit content (activities, programming, logic workflows, puzzles, encryption-decryption etc.), this adds a non-proprietary yet an effective barrier to content piracy<br/><br/>There is also a global leaderboard, the players are awarded points for completing a kit, uploading pictures of their end result with our hashtag to social media platforms. This serves ___ purposes, gives us free social media promotion that looks much more genuine than “This is my product, I gave big bucks to Instagram and now you should buy it” and it creates a competitive spirit that subconsciously tells the kids to buy more kits.<br/><br/>Everytime a kid buys a kit, he/she gets a referral code. This code gives the user an off on the subscription price and the giver more points to top the leaderboard.</p>
            <br/>
            <h4>Market size</h4>
            <p>With the edutainment industry growing bigger than ever with online learning gaining more popularity, it is estimated to be at around $200B globally and about $20B in India itself.</p>
            <br/>
        </div>
    </div>
    <div class="card">
        <div class="width-restriction">
            <h2>The Aesthetics</h2>
            <img src="images/binarybox/aesthetic.png">
        </div>
    </div>
    <div class="card">
        <div class="width-restriction">
            <h2>Thank you for reading this</h2>
            <p>If you wish to work on this project or something similar, feel free to hit us up, see ya!</p>
        </div>
    </div>
    <br/><br/><br/>
</div>