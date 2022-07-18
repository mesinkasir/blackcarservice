<script context="module">
	import data from '../../data/page.json';
    import Car1 from '$lib/fleet/limo1.jpg';
    import Car2 from '$lib/fleet/limo1.webp';
    import Car3 from '$lib/fleet/limo2.jpg';
    import Car4 from '$lib/fleet/limo3.jpg';
</script>
<div class="row">
    <div class="col-md-6 p-3">
        <img class="img-fluid" alt={data.fleettitle} src={Car1}/>
    </div>
    <div class="col-md-6 p-3">
        <img class="img-fluid" alt={data.fleettitle} src={Car2}/>
    </div>
    <div class="col-md-6 p-3">
        <img class="img-fluid" alt={data.fleettitle} src={Car3}/>
    </div>
    <div class="col-md-6 p-3">
        <img class="img-fluid" alt={data.fleettitle} src={Car4}/>
    </div>
</div>