<script context="module">
	import data from '../data/page.json';
	import Fleet from '$lib/fleet/Fleet.svelte';
	import Hero from '$lib/widget/Hero.svelte';
	export const prerender = true;
</script>


<svelte:head>
    <title>{data.fleettitle}</title> 
<meta content='{data.fleettitle}' property='og:title'/>
<meta content='{data.fleettitle} ' name='twitter:title'/>
<meta content='{data.fleettitle}' name='keywords'/>
<meta content='{data.fleettitle}' property='og:site_name'/>
<meta content="{data.fleetdescription}" name="description"/>
<meta content='{data.fleetdescription}' name='twitter:description'/>
<meta content='summary_large_image' name='twitter:card'/>
<meta content={data.twitter} property='twitter:author'/>
<meta content={data.tweet} name='twitter:site'/>
<meta content='{data.cover}' name='twitter:image'/>
<link rel="icon" type="image/x-icon" href="{data.cover}" />
<meta content={data.author} property='og:author'/>
<meta content='website' property='og:type'/>
<meta content='index, follow' name='robots'/>
</svelte:head>

<section>
	<h3>{data.fleettitle}</h3><p>{data.fleetdescription}</p>
<Fleet/><Hero/>
</section>
