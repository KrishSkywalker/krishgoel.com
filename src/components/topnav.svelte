<script>
    import * as animateScroll from "svelte-scrollto";

    let darkMode = true;

    function themeToggle() {
        darkMode = !darkMode;
    }
</script>

<svelte:head>
    {#if !darkMode}
        <link rel="stylesheet" href="light.css">
    {:else}
        <link rel="stylesheet" href="dark.css">
    {/if}
</svelte:head>

<nav>
	<div class="width-restriction">
		<a href="/" class="no-link-effect">
			<h1 id="logo">KRISH GOEL</h1>
		</a>
		<div class="topnav-links">
            <!-- Colour scheme change tings -->
			<a id="theme-toggle" class="no-link-effect" on:click={themeToggle}>
				{#if darkMode}
					🌞
				{:else}
					🌜
				{/if}
            </a>
            <!-- Navigation links -->
			<a href="/blog">✏️ Blog</a>
			<a href="/projects">🌐 Projects</a>
			<a href="/repertoire">📄 Repertoire</a>
			<a href="/experience">🎯 Experience</a>
			<a href="/reachme">☎️ Reach me</a>
		</div>
    </div>
</nav>

<style>
    nav {
        width: 100%;
        
        /* Horizontal scroll */
        white-space: nowrap;
        overflow-x: scroll;
        -webkit-overflow-scrolling: touch;
        -ms-overflow-style: -ms-autohiding-scrollbar;
       
        /* Position */
        position: fixed;
        top: 0px;
       
        /* Style */
        background-color: var(--card-background);
        padding: 10px 0;
        box-shadow: var(--box-shadow);

        z-index: 2;
    }
    nav .topnav-links, nav a {
        display: table-cell;
        vertical-align: middle;
        height: 100%
    }
    nav .topnav-links {
            margin-left: 20vw;
            cursor: default
        }
    @media screen and (min-width: 600px) {
        nav .topnav-links {
            margin-left: 30vw
        }
    }
    nav::-webkit-scrollbar {
        display: none; 
    }
    nav .topnav-links, nav a {
        display: inline-block;
    }
    nav .topnav-links a {
        /* padding-bottom: 5px; */
        /* border-bottom: 1.5px solid rgba(0,0,0,0); */
        /* transition: 0.2s; */
        font-size: 0.9rem;
        margin-right: 10px
    }
    nav .topnav-links a:hover {
        /* border-bottom: 1.5px solid var(--body) */
    }
    nav .topnav-links a {
        padding-right: 10px
    }
    nav .topnav-links #theme-toggle:hover {
        /* border-bottom: 1.5px solid #00000000; */
        cursor: default
    }
</style>