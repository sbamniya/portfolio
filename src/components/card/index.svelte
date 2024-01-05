<script lang="ts">
	export let image: string;
	export let title: string;
	export let description: string;
</script>

<div class="card">
	<img src={image} class="card-img-top image" alt="..." />
	<div class="card-body">
		<div class="card-title">{title}</div>
		<p class="card-text">
			{description}
		</p>
	</div>
</div>

<style scoped lang="scss">
	@import '../../assets/scss/variable';
	.card {
		width: 100%;
		max-width: 370px;
		margin: auto;
		border: none;
		border-radius: 25px;
		overflow: hidden;
		text-align: center;

		.image {
			height: 200px;
		}

		.card-title {
			color: rgba($black, 0.81);
			font-size: $font-18;
			font-family: $poppins-regular;
		}

		.card-text {
			color: rgba($black, 0.5);
			font-weight: 400;
			font-size: $font-14;
			line-height: 22px;
		}
	}
</style>
