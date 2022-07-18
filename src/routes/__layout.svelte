<script>
	import Nav from '$lib/widget/Navi.svelte';
	import Button from '$lib/widget/Button.svelte';
	import Cover from '$lib/widget/Cover.svelte';
	import Header from '$lib/widget/Header.svelte';
	import Footer from '$lib/widget/Footer.svelte';
	import '../app.css';
</script>

<Nav />
<main class="container mt-5">
	<div class="row">
		<div class="col-md-7 p-3 p-md-5">
			<Header/>
		<hr/>
		<Button/>
		<hr/>
		<slot />
	</div>
	<Cover/>
	<Footer/>
</main>
