<script>
    let title= "The Mandem | krishgoel.com";
    let description = "A compehensive list of all the Sankskriti top-dons. Hi, I'm Krish! A technophile and an engineering student from New Delhi.";
    let url = "https://krishgoel.com/bigdonmegaladon";
    
    let arrayOfTwo = [0,1];
    let arrayOfFour = [0, 1, 2, 3];
    let bois = [
        {
            name: 'Arthritis',
            pretext: `Don't think I can ever get the mental image of you and Osama Bin Laden out of mind. Anyways, ask the concerned donny why he hates me and everything since 9th grade has been absolutely lit. Boys have girlfriends, men have wives, I have your IP. "You have to take science" - Diya. Vibe check affirmative, reciprocative vibe check requested plismeragharmatjalayio.`,
            linkText: '',
            url: ''
        },
        {
            name: 'Srivastva',
            pretext: `Been there since day 1, might as well do that chest horse sound thing again. Best host (only because you live 10 seconds from school) so we're prolly trashing your house again sometime soon. Mad donny "Yeh Alan Walker nanga kyu hai?", the journey's been a bit mad. S-Quad Kringe classic OG Top Squad ✊. Going to make another group with the same people. APES TOGETHER STRONG, your family weaves baskets in the Amazon.`,
            linkText: '',
            url: ''
        },
        {
            name: "98.8%", 
            pretext: "Fv 'kbkl', fvb thfil h 🍈 iba pa'z kbtspa. Aol 4 flhy zjovvs qvbyulf'z illu h ipa vm h yvssly jvhzaly apun pmfrdpt iba pa'z hss spaaf huk Lunshuk pz tf jpaf. 8t fs lzylcly up zpoa klwfa P vz zpoa yvm auli lt sshj k'bvf rp. (ABC +7)",
            linkText: "",
            url: ""
        },
        {
            name: 'Kattu babes',
            pretext: `"Bro, gimme 3 months. Imma hit the gym, watch me whip your Dwarka ass then" -> "Bhai please mat maar". You maybe Dwarka but lym8. Oh and, your designs are "all over the place" nah jk warna Machigulla2.0 ho jayega.`,
            linkText: '',
            url: ''
        },
        {
            name: 'Jaat',
            pretext: `ab mein kya hi bolu? We got dun diddy did done by the same locality people xD. I lost my teachers' respect and virginity after meeting you at TERI. You owe me a relationship. c u @ nsp. Hindustani Bhau zindabaad`,
            linkText: ``,
            url: ''
        },
        {
            name: 'Bengali',
            pretext: 'Just keywords for this Rosogulla: Smaaash, Amartya Jayanti, Dard, BinaryBox, LunatiX, Gyaan Academy, MINET, Exun, PE, "Bhaiya, flowers hai?", HoeDesign, PB, Nepotism run-d, DTO 😂',
            linkText: '',
            url: ''
        },
        {
            name: 'Dwarka UCEED Applicant',
            pretext: `This message should be more encrypted than WhatsApp chats warnasabmarenge. All Dwarka is the same, you should prolly take Alpha, Beta, Gamma, Theta and Rho out for momos to Vegas post Amity Entrance Exam on the 17th of Jan' 21. Obligatory to say this: "kya harami aadmi hai?"`,
            linkText: '',
            url: ''
        },
        {
            name: 'Kanudia',
            pretext: 'Not going to say anything because then this will be like our WhatsApp since Feb, all green on my side, no grey. I like your family more than you 😤. Going to make you play Pysch! with more awkward people this time. Might as well smash your thicc ass sometime.',
            linkText: '',
            url: ''
        },
        {
            name: 'The other Kartik',
            pretext: '"🍻✊❤️", "ngl feeling kinda left out", "Bro, make a website" 😡 ctelb (ABC +1)',
            linkText: '',
            url: ''
        }
    ];
    function shuffleArray(array) {
        for (var i = array.length - 1; i > 0; i--) {
            var j = Math.floor(Math.random() * (i + 1));
            var temp = array[i];
            array[i] = array[j];
            array[j] = temp;
        }
    }
    shuffleArray(bois);
</script>

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

<h1>🍻 This one's fr da Sanskriti dons</h1>
<p>Idk when you'll read this but if it's cuz of the yearbook, might as well pop in and say a hi. Just know that if you're mentioned here you should really go kys cuz you spent your time interacting with me in school but this also means you took away a portion of my time and that isn't something I regret giving to any one of you here. ly ❤️</p>
<br/>
<p class="mono">Timestamp: 13th Dec 2020 at 01:59 hrs</p>
<br/>
<p>Also, I'm working on an yearbook app ting rn so if going to 
    <a href="hhtps://yearbook.krishgoel.com" class="mono">yearbook.krishgoel.com</a> 
    doesn't give you an error, go and make a profile there.
</p>
<br/><br/>
<h2>👑 ₹2 Memorial</h2>

<!-- Mobile Screen Layout -->
	<div class="small-screen">
        {#each bois as boi, index}
            <div class="card">
                <div class="width-restriction">
                    <h2>{boi.name}</h2>
                    <p>{boi.pretext}</p>
                    {#if boi.linkText != ""}
                        <a href={boi.url}>🔗 {boi.linkText}</a>
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
                    {#each bois as boi, index}
                        {#if index%2 == i}
                            <div class="card">
                                <div class="width-restriction">
                                    <h2>{boi.name}</h2>
                                    <p>{boi.pretext}</p>
                                    {#if boi.linkText != ""}
                                        <a href={boi.url}>🔗 {boi.linkText}</a>
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
                    {#each bois as boi, index}
                        {#if index%4 == i}
                            <div class="card">
                                <div class="width-restriction">
                                    <h2>{boi.name}</h2>
                                    <p>{boi.pretext}</p>
                                    {#if boi.linkText != ""}
                                        <a href={boi.url}>🔗 {boi.linkText}</a>
                                    {/if}
                                </div>
                            </div>
                        {/if}
                    {/each}
                </div>
            {/each}
        </div>
    </div>