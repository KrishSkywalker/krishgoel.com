<script>
	import Topnav from '../components/common/topnav.svelte';
	import Intro from '../components/index/intro.svelte';
	import Blog from '../components/index/blog.svelte';
	import Projects from '../components/index/projects.svelte';
	import Repertoire from '../components/index/repertoire.svelte';
	import Experience from '../components/index/experience.svelte';
	import ReachMe from '../components/index/reachMe.svelte';
</script>

<style></style>

<svelte:head>
	<title>Krish Goel | KrishSkywalker</title>
</svelte:head>

<Topnav />
<Intro />
<div class="gradient yellow-orange" id="blog"></div>
<Blog />
<div class="gradient orange-purple" id="projects"></div>
<Projects />
<div class="gradient purple-blue" id="repertoire"></div>
<Repertoire />
<div class="gradient blue-fusia" id="experience"></div>
<!-- <Experience /> -->
<!-- <div class="gradient fusia-yellow" id="reachMe"></div> -->
<ReachMe />
<br><br><br><br><br>