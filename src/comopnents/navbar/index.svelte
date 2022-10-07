<script>
	import HireMe from './../hireme/index.svelte';
</script>

<!-- <nav class="navbar navbar-expand-lg">
	<div class="row w-100">
		<div class="collapse navbar-collapse nav-box" id="navbarNav">
			<a class="navbar-brand brand" href="/">Sonu</a>
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
			<ul class="navbar-nav">
				<li class="nav-item">
					<a class="nav-link active" aria-current="page" href="/">About Me</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" aria-current="page" href="/">Services</a>
				</li>

				<li class="nav-item">
					<a class="nav-link " aria-current="page" href="/">Portfolio</a>
				</li>

				<li class="nav-item">
					<a class="nav-link" aria-current="page" href="/">Contact Me</a>
				</li>
			</ul>
			<HireMe />
		</div>
	</div>
</nav> -->
<nav class="navbar navbar-expand-lg fixed-top">
	<div class="container-fluid">
		<a class="navbar-brand brand" href="/">Sonu</a>
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
		<div class="collapse navbar-collapse nav-box" id="navbarSupportedContent">
			<ul class="navbar-nav">
				<li class="nav-item">
					<a class="nav-link active" aria-current="page" href="#about">About Me</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" aria-current="page" href="#services">Services</a>
				</li>

				<li class="nav-item">
					<a class="nav-link " aria-current="page" href="#portfolio">Portfolio</a>
				</li>

				<li class="nav-item">
					<a class="nav-link" aria-current="page" href="#contact">Contact Me</a>
				</li>
			</ul>
			<HireMe />
		</div>
	</div>
</nav>

<style scoped lang="scss">
	@import './../../assets/scss/variable';
	@import './../../assets/scss/mixins';
	.navbar {
		background-color: #fefaf2;
		.nav-box {
			display: flex;
			justify-content: space-between;
			padding: 0;
			@include mq(md) {
				display: none;
			}
			.nav-link {
				text-transform: uppercase;
				cursor: pointer;
			}
			.navbar-nav {
				width: 50%;
				margin: auto;
				justify-content: space-around;
				font-size: $font-14;
			}
		}
		.brand {
			font-family: $logo-font;
			font-size: 50px;
		}
	}
</style>
