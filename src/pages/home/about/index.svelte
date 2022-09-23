<script>
	import AboutText from './about-text.svelte';
	import StandingManIcon from './../../../assets/images/icons/standing-man.svg';
</script>

<section class="row w-100 align-items-center py-5">
	<div class="col-4 col-xs-12 offset-2 d-none d-md-block">
		<img src={StandingManIcon} alt="" class="img-responsive" />
	</div>
	<div class="col-lg-6 col-xs-12">
		<AboutText />
	</div>
</section>

<style scoped lang="scss">
	@import './../../../assets/scss/variable';
</style>
