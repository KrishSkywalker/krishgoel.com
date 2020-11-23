<script>
	import Topnav from '../components/common/topnav.svelte';
</script>


<main>
    <Topnav/>
    <!-- <div class="width-restriction"> --> <!-- Add width-restriction to layout directly -->
        <slot>
        </slot>
    <!-- </div> -->
</main>