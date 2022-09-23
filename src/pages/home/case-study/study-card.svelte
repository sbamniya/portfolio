<script lang="ts">
	export let image: string;
	export let counter: number;
	export let title: string;
	export let description: string;
	export let imagePlacement: 'start' | 'end' = 'start';

	import Button from './../../../comopnents/button/index.svelte';
</script>

<div class="row">
	{#if imagePlacement === 'start'}
		<div class="col-sm-6 col-xs-12">
			<img src={image} alt={image} />
		</div>
	{/if}
	<div class="col-sm-6 col-xs-12">
		<p class="counter">{String(counter).padStart(2, 0)}</p>
		<div class="title">{title}</div>
		<p class="description">{description}</p>
		<Button variant="outline">Details</Button>
	</div>
	{#if imagePlacement === 'end'}
		<div class="col-sm-6 col-xs-12"><img src={image} alt={image} /></div>
	{/if}
</div>

<style scoped lang="scss">
	@import './../../../assets/scss/variable';

	.row {
		margin-top: 50px;
		align-items: center;
		font-family: $poppins-regular;
		.counter {
			color: $primary;
			font-size: 26px;
		}
		.title {
			color: rgba($black, 0.81);
			font-size: 22px;
			font-family: $poppins-regular;
		}
		.description {
			color: rgba($black, 0.5);
			font-size: 16px;
			line-height: 26px;
		}
	}
</style>
