<script>
	import Feedback from './feedback.svelte';
	import Left from './left.svelte';
</script>

<div class="row w-100 align-items-center position-relative py-0 py-sm-5">
	<div class="col-lg-6 col-xs-12">
		<Left />
		<Feedback />
	</div>

	<div class="col-lg-6 text-right d-none d-md-block">
		<img src="/banner-image.png" alt="" />
	</div>
</div>
