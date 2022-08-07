<script>
	import HireMe from './../hireme/index.svelte';
</script>

<nav class="navbar navbar-expand-lg">
	<div class="row w-100">
		<div class="col-4">
			<a class="navbar-brand brand" href="/">Sonu</a>
		</div>
		<div class="col-8">
			<button
				class="navbar-toggler"
				type="button"
				data-bs-toggle="collapse"
				data-bs-target="/navbarNav"
				aria-controls="navbarNav"
				aria-expanded="false"
				aria-label="Toggle navigation"
			>
				<span class="navbar-toggler-icon" />
			</button>
			<div class="collapse navbar-collapse nav-box" id="navbarNav">
				<ul class="navbar-nav">
					<li class="nav-item">
						<a class="nav-link active" aria-current="page" href="/">About Me</a>
					</li>
					<li class="nav-item">
						<a class="nav-link active" aria-current="page" href="/">Services</a>
					</li>

					<li class="nav-item">
						<a class="nav-link active" aria-current="page" href="/">Portfolio</a>
					</li>

					<li class="nav-item">
						<a class="nav-link active" aria-current="page" href="/">Testimonials</a>
					</li>

					<li class="nav-item">
						<a class="nav-link active" aria-current="page" href="/">Contact Me</a>
					</li>
				</ul>
				<HireMe />
			</div>
		</div>
	</div>
</nav>

<style scoped lang="scss">
	@import './../../assets/scss/variable';

	.nav-box {
		display: flex;
		justify-content: space-between;

		.nav-link {
			text-transform: uppercase;
			cursor: pointer;
		}
	}
	.brand {
		font-family: $logo-font;
		font-size: 50px;
	}
	.row {
		align-items: center;
	}
</style>
