<script>
	import * as animateScroll from "svelte-scrollto";

	let darkMode = false;
	function themeToggle() {
        darkMode = !darkMode;
        window.document.body.classList.toggle('dark-mode');
    }
</script>

<style>
	nav {
		width: 100%;
		position: fixed;
		top: 0px;
		padding: 15px 0px;
		background-color: #ffffff;
		box-shadow: rgba(153, 153, 153, 0.89) 7px 7px 21px -10px;
		z-index: 5;
	}
	nav .width-restriction {
		display: flex;
		justify-content: space-between;
		align-items: center;
		white-space: nowrap;
		overflow-x: auto;
		overflow-y:hidden;
	}
	nav #logo {
		padding-right: 30px;
		color: #3a3a3a
	}
	#theme-toggle {
		margin-right: 30px;
		cursor: pointer;
	}
	nav .topnav-links a {
		color: #3a3a3a;
		margin-right: 13px;
		transition: 0.2s;
		font-size: 0.9rem;
		cursor: pointer;
		padding-bottom: 5px;
		border-bottom: 1.5px solid #3a3a3a00;
	}
	nav .topnav-links a:hover {
		border-bottom: 1.5px solid #3a3a3a;
	}
	#theme-toggle:hover {
		border-bottom: none
	}
	:global(body.dark-mode) {
		background-color: #3a3a3a;
		color: #ffffff;
	}	
	:global(body.dark-mode) nav { 
		background-color: #000000;
		box-shadow: 7px 7px 21px -10px rgba(36,36,36,0.89)
	}
	:global(body.dark-mode) nav #logo {
		color: #ffffff;
	}
	:global(body.dark-mode) a {
		color: #ffffff
	}
	/* :global(body.dark-mode) p a {
		color: #ffffff
	} */
	:global(body.dark-mode) nav .topnav-links a:hover {
		border-bottom: 1.5px solid #ffffff;
	}
</style>

<nav>
	<div class="width-restriction">
		<a href="/">
			<h1 id="logo">KRISH GOEL</h1>
		</a>
		<div class="topnav-links">
			<!-- Colour scheme change tings -->
			<a id="theme-toggle" on:click={themeToggle}>
				{#if darkMode}
					🌞
				{:else}
					🌜
				{/if}
			</a>
			<!-- Navigation links -->
			<a href="/blog">✏️ Blog</a>
			<a href="/projects">🌐 Projects</a>
			<a href="/#repertoire">📄 Repertoire</a>
			<a href="/experience">🎯 Experience</a>
			<a href="/reachme">☎️ Reach me</a>
			<!-- <a on:click={() => animateScroll.scrollTo({element: '#blog', offset: -100})}>📝 Blog</a>
			<a on:click={() => animateScroll.scrollTo({element: '#projects', offset: -100})}>🌐 Projects</a>
			<a on:click={() => animateScroll.scrollTo({element: '#repertoire', offset: -100})}>📄 Repertoire</a>
			<a on:click={() => animateScroll.scrollTo({element: '#experience', offset: -100})}>🎯 Experience</a>
			<a on:click={() => animateScroll.scrollTo({element: '#reachMe', offset: -100})}>☎️ Reach me</a> -->
		</div>
	</div>
</nav>