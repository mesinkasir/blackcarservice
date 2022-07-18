<script>
	import Nav from '$lib/widget/Navi.svelte';
	import Menu from '$lib/widget/Menu.svelte';
	import Cover from '$lib/widget/Cover.svelte';
	import Header from '$lib/widget/Header.svelte';
	import Footer from '$lib/widget/Footer.svelte';
	import '../app.css';
</script>

<Nav />
<main class="container mt-5">
	<div class="row">
		<div class="col-md-7 p-3 p-md-5 opacity-75">
			<Header/>
		<hr/>
		<Menu/>
		<hr/>
		<slot />
	</div>
	<Cover/>
	<Footer/>
</main>
