<script context="module">
	import { browser, dev } from '$app/env';
	import data from '../data/page.json';
	import Hero from '$lib/widget/Hero.svelte';
	export const hydrate = dev;
	export const router = browser;
	export const prerender = true;
</script>

<svelte:head>
		<title>{data.abouttitle}</title> 
<meta content='{data.abouttitle}' property='og:title'/>
<meta content='{data.abouttitle} ' name='twitter:title'/>
<meta content='{data.abouttitle}' name='keywords'/>
<meta content='{data.abouttitle}' property='og:site_name'/>
<meta content="{data.abouttext1}" name="description"/>
<meta content='{data.abouttext1}' name='twitter:description'/>
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
	<p>{data.abouttext1}</p><p>{data.abouttext2} <a href="https://kit.svelte.dev">Sveltekit</a> feat <a href="https://vitejs.dev/">Vite</a> {data.abouttext2a}</p>
	<p>{data.abouttext3}</p><p>{data.abouttext4}</p><p><a href="/about">Black Car Service Website</a> {data.abouttext5}</p><Hero/>
</section>
