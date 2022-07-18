<script context="module">
	import data from '../../data/page.json';
</script>
<div class="border-top row border-secondary">
	<div class="col-md-9 p-3 p-md-5">
	<h3 class="display-1"><a href={data.url}>{data.title}</a></h3>
	</div>
	<div class="col-md-3 p-3 p-md-5 lead">
	<p>{data.address}<br/>{data.phone}<br/>{data.email}</p>
</div>
</div>