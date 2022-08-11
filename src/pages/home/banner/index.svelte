<script>
	import Feedback from './feedback.svelte';
	import Left from './left.svelte';
</script>

<div class="row w-100 align-items-center position-relative">
	<div class="col-6  col-xs-12">
		<Left />
		<br />
		<Feedback />
	</div>

	<div class="col-6 text-right d-xs-none">
		<img src="/banner-image.png" alt="" />
	</div>
</div>
