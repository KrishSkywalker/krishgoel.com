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
    .card a {
        border-bottom: 1.5px solid #ffffff;
        transition: 0.2s;
        padding-bottom: 5px;
        font-size: 0.9rem
    }
    .card a:hover {
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
    let arrayOfTwo = [0,1];
    let arrayOfFour = [0, 1, 2, 3];
    let experienceCards = [
		{
            title: "India's Super Brain", 
            subhead: "September 2020",
            pretext: "I completed the India's Super Brain event, a 4 week long workshop-cum-challenge. The idea was to teach a new language each week, from ReactJS and DBM to cybersecurity and Machine Learning. It gave me a good intro to all these subdomains.",
            linkText: "",
            url: ""
        },
        {
            title: "Pitch @ MINET X", 
            subhead: "🏆 Placed #2 | September 2020",
            pretext: "Amartya, Kataria and I worked on an online education startup for what can essentially be called a fancy hackathon and bagged the 2nd position. This is personally my favourite dub because this was practically my last interschool IT event and it couldn't have been better.",
            linkText: "minet.co",
            url: "https://minet.co"
        },
        {
            title: "CryptX @ MINET X 2020", 
            subhead: "🏆 Placed #3 | September 2020",
            pretext: "As a club, we took it as a challenge to atleast be in the top 3 for this hunt and went all in. The #3 dub really boosted our morale for the events to follow.",
            linkText: "cryptx.co",
            url: "https://cryptx.co/leaderboard/"
        },
        {
            title: "BetaTest", 
            subhead: "Handler | August 2020",
            pretext: "We went classic input-box with the second edition of ProjectBeta's infamous cryptic hunt, while we didn't suffer any DDoS attacks, our servers went offline regularly. Even though the event wasn't the smoothest, we learnt a lot about handling a real life crisis.",
            linkText: "BetaTest Portal",
            url: "https://projectbeta.xyz"
        },
        {
            title: "ReapBenefit COVID-19 Division Fundraiser", 
            subhead: "July 2020",
            pretext: "I was involved with ReapBenefit COVID-19 Division, a student led initiative in collaboration with ReapBenefit Solve Ninjas. The aim was to assist 39 families of the Gosavi community in the Hubli district of Karnataka. We raised a grand total of $650.",
            linkText: "Fundraising website",
            url: "https://reapbenefitfundraiser.herokuapp.com/"
        },
        {
            title: "Webinar on AI", 
            subhead: "July 2020",
            pretext: "Raghav Sarangi and I (along with 2 teachers and Mr. Arya Nagar) delivered a 2 hour webinar on Artificial Intelligence and its relevance in today's world for all the 280 teachers at Sanskriti School. We recieved an extremely positive feedback.",
            linkText: "",
            url: ""
        },
        {
            title: "Cryptic Hunt @ Quarantech", 
            subhead: "🏆 Placed #2 | June 2020",
            pretext: "Parth Sarthi and I participated in an online tech event organized by a school and placed #2 in the 48 hours cryptic hunt event out of the 20 competing teams.",
            linkText: "",
            url: ""
        },
        {
            title: "Wellfur Foundation", 
            subhead: "May 2020",
            pretext: "I recently helped Wellfur Foundation, a student led organization working towards helping street animals by feeding them and providing them with medical care and attention.",
            linkText: "Wellfur Foundation Webapp",
            url: "https://wellfurfoundation.herokuapp.com/"
        },
        {
            title: "Web Dev & Python Worksop", 
            subhead: "April - May 2020",
            pretext: "Amidst the COVID-19 lockdown, I conducted the second round of my web development and Python workshop with 17 students gratis to ensure that the kids don't get bored and learn something helpful.",
            linkText: "",
            url: ""
        },
        {
            title: "ProjectBeta", 
            subhead: "Head of AI and IoT 2020",
            pretext: "I was selected as the head of department for AI and IoT for the academic session 2020-21.",
            linkText: "projectbeta.tech",
            url: "http://projectbeta.tech"
        },
        {
            title: "Sanskriti MUN 2019", 
            subhead: "Director of TechOps | December 2019",
            pretext: "I was the Director of TechOps at Sanskriti School Intra Model United Nations 2019. My work included developing a website that could be used for the future installments of the event and all the technological aid required to ensure a smooth experience throughout the conference.",
            linkText: "sanskritimun.com",
            url: "https://sanskritimun.com"
        },
        {
            title: "SpaceTech @ Exun", 
            subhead: "October 2019",
            pretext: "Kartik Gupta, Raghav Sarangi and I developed an idea for agricultural growth on the Lunar surface. While the idea did stand out, we couldn't make it to top 3 because of our technological contingencies. You can read on the idea below.",
            linkText: "LunatiX Documentation",
            url: "https://drive.google.com/drive/folders/1E7EJTsJhww2c5vz1DRLYnc9JRg6RynOU?usp=sharing"
        },
        {
            title: "BetaTest", 
            subhead: "Handler | October 2019",
            pretext: "Organised and planned the infamous CTF cryptic hunt for ProjectBeta 3.0 2019. The participants had an extremely positive review about the same.",
            linkText: "",
            url: ""
        },
        {
            title: "Pitch @ MINET X", 
            subhead: "🏆 Placed #3 | September 2019",
            pretext: "Kartik Gupta and I developed our STEM education startup BinaryBox. You can read more about it in the projects section above. We successfully raised $100K out of the available $500K post qualifying for the make league.",
            linkText: "minet.co",
            url: "https://minet.co/"
        },
        {
            title: "ProjectBeta", 
            subhead: "Vice President 2019",
            pretext: "I served as the Vice-President and Head of AI and IoT at my school's IT club - ProjectBeta. I led the teams in various interschool startup events including programming, pitch and design.",
            linkText: "projectbeta.tech",
            url: "http://projectbeta.tech"
        },
        {
            title: "Sanskriti MUN 2019", 
            subhead: "Additional Director of Tech Ops | April 2019",
            pretext: "I was the Additional Director of TechOps at Sanskriti School Model United Nations 2019. My work included graphic designing and all the technological aid required to ensure a smooth experience throughout the conference.",
            linkText: "sanskritimun.com",
            url: "https://sanskritimun.com/"
        },
        {
            title: "Web Dev Worksop", 
            subhead: "June 2018",
            pretext: "Organised and conducted a three-week summer workshop on web development and logic development through Scratch for the younger students. This not only gave me an opportunity to give back to the society but also helped me earn some pocket money respectfully.",
            linkText: "",
            url: ""
        },
        {
            title: "Bliss IoT Luxury", 
            subhead: "Interned 2015-17",
            pretext: "With Bliss, we aimed at developing a luxurious watch with everything you'll find in a Rolex while combining it with smartness far greater than any of the current smartwatches. This is where I really felt the spark that pushed me into the technological domain.",
            linkText: "blisswatches.com",
            url: "https://blisswatches.com/"
        },
        {
            title: "ASSET DukeTip Scholarship", 
            subhead: "Qualified for the Duke University scholarship",
            pretext: "I was placed among the top 5% students among India and UAE and hence chosen for the summer programme at Duke University, Durham.",
            linkText: "Asset DukeTip",
            url: "https://tip.duke.edu/programs/estudies/application-instructions/international-students"
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
                                    {#if experience.linkText != ""}
                                        <a href={experience.url}>🔗 {experience.linkText}</a>
                                    {/if}
                                </div>
                            </div>
                        {/if}
                    {/each}
                </div>
            {/each}
        </div>
    </div>

</div>