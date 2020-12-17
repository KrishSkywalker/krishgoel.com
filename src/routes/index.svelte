<script>
    import Intro from '../components/intro-section.svelte'
    import Blog from '../components/blog-section.svelte'
    import Projects from '../components/projects-section.svelte'
    // import Repertoire from '../components/repertoire-section.svelte'
    import ReachMe from '../components/reachme-section.svelte'

    let title="Krish Goel | KrishSkywalker";
    let description = "Hi, I'm Krish! A technophile and an engineering student from New Delhi. I aspire to develop ‘smarter’ energy sources with the lines I type.";
    let url = "https://krishgoel.com";

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

<Intro/>
<!-- <div class="gradient yellow-orange" id="blog"></div>
<Blog /> -->
<div class="gradient orange-purple" id="projects"></div>
<Projects />
<div class="gradient purple-blue" id="repertoire"></div>
<!-- <Repertoire /> -->
<!-- <div class="gradient blue-fusia" id="experience"></div> -->
<ReachMe />