<script>
	import AboutText from './about-text.svelte';
	import StandingManIcon from './../../../assets/images/icons/standing-man.svg';
</script>

<div class="row w-100 align-items-center">
	<div class="col-4 col-xs-12 offset-2">
		<img src={StandingManIcon} alt="" class="img-responsive" />
	</div>
	<div class="col-6 col-xs-12">
		<AboutText />
	</div>
</div>

<style scoped lang="scss">
	@import './../../../assets/scss/variable';
</style>
