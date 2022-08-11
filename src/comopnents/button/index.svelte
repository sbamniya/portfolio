<script lang="ts">
	export let variant: 'default' | 'icon' | 'outline' = 'default';
</script>

<button
	class="btn btn-primary"
	class:icon={variant === 'icon'}
	class:outline={variant === 'outline'}
>
	<slot />
</button>

<style scoped lang="scss">
	@import './../../assets/scss//variable';
	.btn {
		color: $white;
		min-width: 120px;
		padding: 10px;

		&.icon {
			background-color: unset;
			color: $black;
			border: none;
		}

		&.outline {
			background-color: unset;
			border: 1px solid $primary;
			color: $primary;

			&:hover {
				background-color: $primary;
				color: $white;
			}
		}
	}
</style>
