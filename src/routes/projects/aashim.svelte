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
                The Gyaan Academy is our idea submission to the to solve not just 1 but all 17 Sustainable Development Goals. When we set out on our journey to build this idea ground-up, our goal wasn't to win but to create, build something novel that could really be scaled to not just India but any region of the world, to make quality education more accessible.
                <br/><br/>
                Personally, we've have always been passionate about changing the education system for good, teaching what's useful, what the student wants to learn and teaching to the point of perfection. While it is one of our life goals to build a school with the best in class infrastructure and state of the art curriculum, this competition gave us a chance to rethink all of that. Why do it then, why not now? Why only for the 3,000 kids who'll attend and not the millions who can do it online? Why only for the ones who'll be able to afford it? Why not everyone who deserves it? The Gyaan Academy answered all of that.
                <br/>
            </p>
        </div>
    </div>

    <!-- What is the Gyaan Academy? -->
    <div class="card">
        <div class="width-restriction">
            <h2>What is the Gyaan Academy?</h2>
            <br/>
            <div class="col-container">
                <div class="col-2">
                    <img src="images/gyaanacademy/deck/1.png">
                </div>
                <div class="col-2">
                    <img src="images/gyaanacademy/deck/2.png">
                </div>
            </div>
            <br/>
            <p>The Gyaan Academy isn't just another Udemy, it’s the new social network. While searching for solutions, we realised that every sustainable dev goal is a subset of the bigger problem - that lack of an educated population so, targeting this root cause would essentially mean eventually minimizing the others. Mahatama Gandhi described education as the mightiest means to shake the world, gently and that's where our thoughts coincided.</p>
        </div>
    </div>

    <!-- USPs -->
    <div class="card">
        <div class="width-restriction">
            <!-- <h2></h2> -->
            <img src="images/gyaanacademy/deck/3.png">
            <br/><br/>
            <h4>Learning what that matters more</h4>
            <p>The things we wanted to learn were never a part of the school syllabus or the content was inadequate, things like entrepreneurship, programming, culinary arts, financial education, even growing plants and hydroponics weren’t there and we believe they would have been much more helpful to us than the history lessons. Well, we don’t do that here, you’re taught only what you want to learn and to the point of perfection.<br/>
            Being strong believers of Ikigai, we wanted our course selection algos and support to help you find yours.</p>
            <h4>Learning from the best, the masters of the trade</h4>
            <p> You choose your gurus and learn from the industry experts, you learn concepts that you can apply in the real world, concepts that are relevant, you design your own future and you learn from the master because obviously, learning from the masters comes with it added extra benefits.</p>
            <h4>Building the connections you'd build in a school</h4>
            <p>We understand the importance of having real people in your life and the fact that everyone loves a little highschool drama and would definitely not want you to be deprived of that, so unlike other learning platforms where you just pursue courses, with Gyaan, you do the same but with friends. The platform has groups, mostly categorised on the basis of your age and organises regular meetups and other bonding activities.</p>
        </div>
    </div>

    <!-- How we make it happen -->
    <div class="card">
        <div class="width-restriction">
            <h2>How we make it happen</h2>
            <br/>
            <img src="images/gyaanacademy/deck/4.png">
            <br/>
            <div class="col-container">
                <div class="col-2">
                    <img src="images/gyaanacademy/deck/5.png">
                    <h4>Life Skills Development</h4>
                    <p style="width: 95%">
                        First up, we have SUPW Education or Vocational Education and we don’t just restrict ourselves to SUPW, we call it life skills development.
                        <br/>
                        Someone said, an ounce of theory is worth a ton of action and we couldn;t agree more. When the human brain learns by doing, it learns outside the “ideal-scenario” bubble, it learns where things go wrong and learns the importance of failure for Yoda said, “The greatest teacher failure is”
                    </p>
                    <br/>
                </div>
                <div class="col-2">
                    <img src="images/gyaanacademy/deck/6.png">
                    <h4>Master Classes</h4>
                    <p style="width: 95%">While we don’t really have much to explain here, learning from the master of your trade obviously comes with its own set of benefits, think about it this way, would you wanna be mentored by someone who’s only well versed with theory or someone like Stephen Hawking.</p>
                </div>
            </div>
            <div class="col-container">
                <div class="col-2">
                    <img src="images/gyaanacademy/deck/7.png">
                    <h4 style="width: 95%">Curriculum designed with child psychologists and experts</h4>
                    <p style="width: 95%">We work with the professionals and child psychologists to make sure you learn what is needed without stressing your brains out, to make learning fun while ensuring no one gets bored. This curriculum is periodically updated to prevent any redundancy in terms of content and goes without saying, we add new career and professions continuously.</p>
                </div>
                <div class="col-2">
                    <img src="images/gyaanacademy/deck/8.png">
                    <h4>Creating social connections</h4>
                    <p style="width: 95%">I am sure all of us would agree, school isn’t defined by the 5 subjects taught, it’s about the people, about the friends and about the fun times and nothing could make us deprive you of it so we make sure you develop the same social connections as you would in a physical school. With intra and inter school events, meetups, bonding activities etc.</p>
                </div>
            </div>
        </div>
    </div>

    <!-- Seekho-Sikhao Programme -->
    <div class="card">
        <div class="width-restriction">
            <h2>Making it more accessible: The Seekho-Sikhao Programme</h2>
            <br/>
            <img src="images/gyaanacademy/deck/9.png">
            <br/>
            <p>
                Coming to, what about the rural, remote areas and the economically backwards sections of the society? Bill Gates said that it isn’t your fault if you’re born poor, it is if you die poor, with our Seekho-Sikhao Programme, we’ll be ensuring our level best that we don’t let the poor die poor.
                <br/><br/>The idea of this community outreach programme is to educate the people in the remote areas and we’re not talking about programming but about skills that’ll be particularly helpful to them, like operating a computer, technologies to advance their current livelihood, hydroponics and other activities for farmers, basic math, english and science education for the school kids by partnering up with the local schools etc.
                <br/><br/>And all of this is done by volunteers from our userbase under the guidance of our mentors and masters, at the end of each of these workshops, you receive a certificate or achievement and the pride of giving back to the community you take so much from.
            </p>
        </div>
    </div>

    <!-- Plan of Expansion -->
    <div class="card">
        <div class="width-restriction">
            <h2>The Plan of Expansion: Plan 2.0</h2>
            <div class="col-container">
                <div class="col-2">
                    <img src="images/gyaanacademy/deck/10.png">
                </div>
                <div class="col-2">
                    <img src="images/gyaanacademy/deck/11.png">
                </div>
            </div>
            <h4>AR/VR Integration</h4>
            <p>Imagine being able to get a tour of your dream IT company, your favourite automobile brand’s factory, a modern day hydroponics farm or Gordon Ramsey’s kitchen all with your friends from the comfort of your homes. That’s all a part of our AR/VR implementation plan.</p>
            <h4>The world's headed towards social commerce and so are we</h4>
            <p>Gyaan Academy isn’t just a school, it’s the new learning social media platform. To explain this aspect in a little more details, let’s imagine a scenario where you open Instagram and scroll through your feed to see your friends showcasing their achievements, taking courses, master classes going on, even you teaching i.e. any user passing certain requirements to start a course and teach a skill to everyone else around, that’s what our vision coincides with.</p>
            <h4>Real life school collaborations</h4>
            <p>And after a certain period of time and gaining credibility, we also plan on having Gyaan Academy divisions in school and other educational institutes, all integrated with our APIs because our vision isn't to put the current learning systems out of business but to enhance them.</p>
        </div>
    </div>

    <!-- Econ and Model -->
    <div class="card">
        <div class="width-restriction">
            <h2>The econ and the business model</h2>
            <br/>
            <img src="images/gyaanacademy/deck/12.png">
            <div class="col-container">
                <div class="col-2">
                    <img src="images/gyaanacademy/deck/13.png">
                </div>
                <div class="col-2">
                    <img src="images/gyaanacademy/deck/14.png">
                </div>
            </div>
            <br/>
            <p>
                Now comes the part about economics and the funds usage.  Our goal isn’t just to make a strong economy, it’s to make a beautiful, a sundar one. While the majority of the funds would go into making the content and development of the tech stack, we’d also need funds for advertisements and promotions. Which I'll be talking about in the coming sections.
                <br/><br/>
                Another strat that can be implemented is paying the master educators for the core initial courses in course royalty fees which may or may not be capped.
                <br/><br/>
                Our money-model approach is extremely simple, take the money from the user and pay our bills just as any other business. The interesting part comes in when we talk about the funds usage and the membership plans.
                <br/>
                We plan on offering 2 options of the end consumer - buying a course or buying a subscription. While buying a course is similar to our pseudo-competitors like CourseEra and Udemy, the latter i.e. our subscription model is what that sets up apart. The subscription allows you the access to all of our ‘smarter’ features which includes all of the schooling experience for a limited time much like you’d expect in a school.
                <br/>
                To put it into perspective, it’s much like the Kindle books model, you can either buy a book for a price or you can get the KindleUnlimited subscription where you get access to a large library for a llimited time.
                <br/><br/>
                Now, being an avid reader, The $100 Startup by Chris Guillebeau taught me that any business runs on how it adds value to itself and the user, while the users learn and become a better version of themselves, we add value to ourselves not just throught the monetary transactions of $15-$20 a month, we do it because we create a network, a network of people willing to learn, the next generation which will be the next set of change makers, once we tap that network, the wealth will have no upper cap. Because the only basic fundamental law to run a business is miniaml expenditure and maximum influx of the green, when we have the access to such a network, the marketing costs (also the main expense) drops to absolute minimal 'cause the network does the promotion for us and that's just one way to look at it.
                <br/><br/>
                Milan Kundera said , "A busines has only 2 aspects, innovation and marketing. So while we have the innovation part nailed down, let's talk about marketing, about getting the word out there and about changing the education system around the world for good.
                <br/>
                It’s the 21st century and we can’t possibly rely on billboards so we’ll be implementing smart promotion strategies like competitive leaderboards, targeted social media ads with smart analytics, rewards for posting and sharing the platform and achievements.
                <br/><br/>
                As suggested by Mr. Aryaman, our mentor for The Gyan Acad, we could really implement acquisition marketing  i.e. using smart methods to acquire targeted customers who are already slightly inclined into buying your services instead of trying to approach the open world and trying to get everyone, even the people who wouldn't be even remotely interested.
                <br/><br/>
                Our stratergies for customer acquisition would mainly revolve around social media resharing, why do we buy sneakers? They look good yes but a lot of it comes from the fact that your friends have it too, it makes you feel like a part of a group, we aim at creating a similar feelng  of belongingness with our social media campaign, much like people use Instagram because their friends are there, we want people to use TGA because their friends are learning with us. 
                Bonus social media content would include special filters, badges that people can share on their profiles, even if they aren't a customer, we want to create an experience that they can cherish even without paying us and here's how it benefits us, when they use our filters, they essentially promote us and that gentlement, is social media commerce for you. That's what we plan to do.
            </p>
        </div>
    </div>

    <!-- User engagment -->
    <div class="card">
        <div class="width-restriction">
            <h2>Ensuring user engagement</h2>
            <p>Because kids have the attention span of a 2 year old</p>
            <br/>
            <img src="images/gyaanacademy/deck/15.png">
            <br/>
            <p>
                <span class="bold">Another point raised was, how do we keep the user involved, especially kids who lack the concentration required?</span>
                <br/><br/>
                While our core strategy would to be have engaging teaching techniques but that obviously isn't enough so we'll be gamifying the whole process. The user will get point for achievements, completing courses, learning, engaging with other users, referring other users etc. This is bound to create the feeling of healthy competition, the leaderboard will be available at various divisions starting from 'Your Friends' to 'Global'. Other techniques include social media platform integrations with Instagram and Snapchat because this is Gen-Z.
            </p>
        </div>
    </div>

    <!-- Tech stack -->
    <div class="card">
        <div class="width-restriction">
            <h2>The Tech Stack</h2>
            <p>Because at the end of it, it's a tech startup</p>
            <br/>
            <img src="images/gyaanacademy/deck/16.png">
            <br/><br/>
            <p>
                While there isn't much to talk the tech stack here since this is an idea pitch but no harm in briefing, so for minimal expenditure we'll be going for a PWA initially built on Vue.JS with MongoDB and host it on Heroku or Vercel for functional and smooth cross-platform support. But since nothing beats an old fashioned mobile application so later on we'll be working on developing those.
            </p>
        </div>
    </div>

    <!-- Thankyou -->
    <div class="card">
        <div class="width-restriction">
            <h2>Thank you for reading this</h2>
            <p>If you wish to work on this project or something similar, feel free to hit us up, see ya!</p>
            <br/>
            <img src="images/gyaanacademy/designdeck/13.png">
        </div>
    </div>
    <br/><br/><br/>
</div>