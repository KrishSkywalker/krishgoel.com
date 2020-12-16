<script>
    import Topnav from '../components/topnav.svelte';
</script>

<main>
    <Topnav/>
    <br/><br/><br/><br/><br/>
    <div class="width-restriction">
        <slot>
        </slot>
    </div>
    <br/><br/><br/><br/><br/>
</main>