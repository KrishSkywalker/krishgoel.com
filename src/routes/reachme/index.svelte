<script>
    let title= "Reach Me | krishgoel.com";
    let description = "Feel free to hit me up, all the pathways are mentioned here. Hi, I'm Krish! A technophile and an engineering student from New Delhi.";
    let url = "https://krishgoel.com/reachme";

    import ReachMe from "../../components/reachme-section.svelte"
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

<ReachMe/>