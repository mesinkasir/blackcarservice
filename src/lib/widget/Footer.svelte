<script context="module">
	import data from '../../data/page.json';
</script>
<div class="border-top row border-secondary opacity-75">
	<div class="col-md-9 p-3 p-md-5 opacity-75">
	<h3 class="display-1"><a href={data.url}>{data.title}</a></h3>
	</div>
	<div class="col-md-3 p-3 p-md-5 opacity-75 lead">
	<p>{data.address}<br/>{data.phone}<br/>{data.email}</p>
</div>
</div>