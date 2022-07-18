<script context="module">
	import data from '../data/page.json';
	import Hero from '$lib/widget/Hero.svelte';
    let title= 'Black car service limousine car rental website creation - web development';
    let description = '';
    let blackcar = 'Black Car Premium PRO Version →';
    let blackurl = 'https://blackcar.axcora.com';
    let cybercar = 'Cyber Car Website Template PRO →';
    let cyberurl = 'https://cybercar.vercel.app';
    let limoweb = 'Limousine website PRO Version →';
    let limourl = 'https://limoweb.vercel.app/';
	export const prerender = true;
</script>


<svelte:head>
    <title>{data.title}</title> 
<meta content='{title}' property='og:title'/>
<meta content='{title} ' name='twitter:title'/>
<meta content='{title}' name='keywords'/>
<meta content='{title}' property='og:site_name'/>
<meta content="{description}" name="description"/>
<meta content='{description}' name='twitter:description'/>
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
	<h3><a href={data.menu4}>{title}</a></h3><p>{data.protext1}</p><p>{data.protext2}</p><p>{data.protext3}</p>
    <h5><a href={blackurl}>{blackcar}</a></h5><h5><a href={cyberurl}>{cybercar}</a></h5><h5><a href={limourl}>{limoweb}</a></h5>
    <p>{data.protext4}</p><Hero/>
</section>
