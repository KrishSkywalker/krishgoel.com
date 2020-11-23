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
    .center a {
        color: #3a3a3a;
        border-bottom: 1.5px solid #ffffff;
        transition: 0.2s;
        padding-bottom: 10px
    }
    .center a:hover {
        border-bottom-color: #3a3a3a;
    }
    .card .social-media-links a {
        padding-bottom: 10px;
        border-bottom: 1.5px solid #ffffff;
        transition: 0.2s;
        /* display: inline-block; */
        padding: 0px 5px;
        padding-bottom: 10px;
        border-bottom: 1.5px solid #ffffff;
        margin-top: 15px;
        transition: 0.2s;
        display: -webkit-box;
        display: flex;
        -webkit-box-pack: center;
        justify-content: center;
        -webkit-box-align: center;
        align-items: center;
        display: inline-block;
    }
    .card a:hover {
        border-bottom: 1.5px solid #3a3a3a;
    }
    .card .social-media-links img {
        vertical-align: middle;
        border-radius: 0px; 
        width: 20px;
        padding-right: 3px;
    }
    .card .social-media-links #github-light {
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
    :global(body.dark-mode) .card a {
        border-bottom-color: #000000;
    }
    :global(body.dark-mode) .card a:hover {
        border-bottom-color: #ffffff;
    }
    :global(body.dark-mode) .card .social-media-links a #github-dark {
        display: none
    }
    :global(body.dark-mode) .card .social-media-links a #github-light {
        display: inline-block
    }
    :global(body.dark-mode) .center a {
        color: #ffffff;
        border-bottom-color: #3a3a3a00;
    }
    :global(body.dark-mode) .center a:hover {
        border-bottom-color: #ffffff;
    }
</style>

<script>
    import ReachMe from '../../components/common/reachMe.svelte';
</script>

<svelte:head>
	<title>Reach Me | krishgoel.com</title>
</svelte:head>

<br><br><br><br><br><br>

<ReachMe/>

<br/><br/><br/>