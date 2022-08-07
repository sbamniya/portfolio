<script>
	import Feedback from './feedback.svelte';
	import Left from './left.svelte';
</script>

<div class="row w-100 align-items-center position-relative">
	<div class="col-6">
		<Left />
	</div>

	<div class="col-6 text-right">
		<img src="/banner-image.png" alt="" />
	</div>
	<Feedback />
</div>
