<script lang="ts">
	export let variant: 'default' | 'icon' = 'default';
</script>

<button class="btn btn-primary" class:icon={variant === 'icon'}>
	<slot />
</button>

<style scoped lang="scss">
	@import './../../assets/scss//variable';
	.btn {
		color: #fff;
		min-width: 120px;
		padding: 10px;

		&.icon {
			background-color: unset;
			color: $black;
			border: none;
		}
	}
</style>
