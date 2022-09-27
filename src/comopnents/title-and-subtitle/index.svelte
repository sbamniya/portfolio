<script lang="ts">
	export let title: string;
	export let subTitle: string;
</script>

<div class="text-center">
	<p class="heading">{title}</p>
	<h4 class="title">{subTitle}</h4>
</div>

<style lang="scss" scoped>
	@import './../../assets/scss/variable';

	.heading {
		color: $primary;
		text-transform: uppercase;
		font-size: $font-22;
		font-family: $poppins-regular;
		margin: 0;
	}
	.title {
		color: rgba($black, 0.81);
		font-size: $font-28;
		font-weight: 600;
		font-family: $poppins-regular;
	}
</style>
