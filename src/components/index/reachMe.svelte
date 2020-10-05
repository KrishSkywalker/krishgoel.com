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

    .card .social-media-links a {
        /* display: inline-block; */
        padding: 0px 5px;
        padding-bottom: 10px;
        margin-top: 15px;
        border-bottom: 1.5px solid #ffffff;
        transition: 0.2s;
        display: -webkit-box;
        display: flex;
        -webkit-box-pack: center;
        justify-content: center;
        -webkit-box-align: center;
        align-items: center;
        display: inline-block;
    }
    .card .social-media-links a:hover {
        border-bottom: 1.5px solid #3a3a3a;
    }
    .card .social-media-links img {
        vertical-align: middle;
        border-radius: 0px; 
        width: 20px;
        padding-right: 3px;
    }
    .card .social-media-links a #github-light {
        display: none;
    }

    :global(body.dark-mode) .card {
        background-color: #000000;
        box-shadow: rgba(36, 36, 36, 0.89) 7px 7px 21px -10px;
    }
    :global(body.dark-mode) .card p a {
        color: #ffffff
    }
    :global(body.dark-mode) .card a {
        color: #ffffff
    }
    :global(body.dark-mode) .card .social-media-links a {
        border-bottom-color: #000000;
    }
    :global(body.dark-mode) .card .social-media-links a:hover {
        border-bottom-color: #ffffff;
    }
    :global(body.dark-mode) .card .social-media-links a #github-dark {
        display: none
    }
    :global(body.dark-mode) .card .social-media-links a #github-light {
        display: block
    }
</style>

<script></script>

<div class="width-restriction">
    <h1 class="mono">☎️ Reach me</h1>
    
    <div class="small-screen">
        <div class="card" style="background-color: #000000">
            <div class="width-restriction">
                <iframe class="spotify" src="https://open.spotify.com/embed/playlist/26Dig7gzJrw1Cqm8sgHI5f" width="100%" height="500px" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
            </div>
        </div>
        <div class="card">
            <div class="width-restriction">
                <p>Feel free to hit me up on any of these platforms</p>
                <div class="social-media-links">
                    <a href="#">
                        <img src="images/icons/instagram.svg">
                        Instagram
                    </a>
                    <a href="#">
                        <img src="images/icons/twitter.svg">
                        Twitter
                    </a>
                    <a href="#">
                        <img src="images/icons/github.svg" id="github-dark">
                        <img src="images/icons/github-light.svg" id="github-light">
                        Github
                    </a>
                    <a href="#">
                        <img src="images/icons/gmail.svg">
                        Mail
                    </a>
                    <a href="#">
                        <img src="images/icons/linkedin.svg">
                        LinkedIn
                    </a>
                    <a href="#">
                        <img src="images/icons/spotify.svg">
                        Spotify
                    </a>
                    <a href="#">
                        <img src="images/icons/reddit.svg">
                        Reddit
                    </a>
                </div>
            </div>
        </div>
        <div class="gradient yellow-cyan"></div>
        <p class="center bold">May the force be with you!<br><br>
            Made with ❤️ and some code
        </p>
    </div>

    <div class="large-screen">
        <div class="col-container">
            <div class="col-2">
                <div class="card" style="background-color: #000000">
                    <div class="width-restriction">
                        <iframe class="spotify" src="https://open.spotify.com/embed/playlist/26Dig7gzJrw1Cqm8sgHI5f" width="100%" height="500px" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
                    </div>
                </div>
            </div>
            <div class="col-2">
                <div class="card">
                    <div class="width-restriction">
                        <p>Feel free to hit me up on any of these platforms</p>
                        <div class="social-media-links">
                            <a href="#">
                                <img src="images/icons/instagram.svg">
                                Instagram
                            </a>
                            <a href="#">
                                <img src="images/icons/twitter.svg">
                                Twitter
                            </a>
                            <a href="#">
                                <img src="images/icons/github.svg" id="github-dark">
                                <img src="images/icons/github-light.svg" id="github-light">
                                Github
                            </a>
                            <a href="#">
                                <img src="images/icons/gmail.svg">
                                Mail
                            </a>
                            <a href="#">
                                <img src="images/icons/linkedin.svg">
                                LinkedIn
                            </a>
                            <a href="#">
                                <img src="images/icons/spotify.svg">
                                Spotify
                            </a>
                            <a href="#">
                                <img src="images/icons/reddit.svg">
                                Reddit
                            </a>
                        </div>
                    </div>
                </div>
                <div class="gradient yellow-cyan"></div>
                <p class="center bold">May the force be with you!<br><br>
                    Made with ❤️ and some code
                </p>
            </div>
        </div>
    </div>
</div>