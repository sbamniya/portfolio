<script lang="ts">
	import TitleAndSubtitle from './../../../comopnents/title-and-subtitle/index.svelte';
	import profile from '../../../assets/images/profile.png';
	// import Carousel from 'svelte-carousel';
</script>

<section class="testimonial-container py-5">
	<TitleAndSubtitle title="TESTIMONIALS" subTitle="What People Says" />
	<div class="row pt-5">
		<div id="carouselExampleDark" class="carousel carousel-dark slide" data-bs-ride="carousel">
			<div class="left-background" />
			<div class="right-background" />
			<!-- <div class="carousel-indicators">
					<button
						type="button"
						data-bs-target="#carouselExampleDark"
						data-bs-slide-to="0"
						class="active"
						aria-current="true"
						aria-label="Slide 1"
					/>
					<button
						type="button"
						data-bs-target="#carouselExampleDark"
						data-bs-slide-to="1"
						aria-label="Slide 2"
					/>
					<button
						type="button"
						data-bs-target="#carouselExampleDark"
						data-bs-slide-to="2"
						aria-label="Slide 3"
					/>
				</div> -->
			<div class="carousel-inner">
				<div class="carousel-item active" data-bs-interval="10000">
					<div class="slide-section">
						<div class="textSection">
							<img src={profile} alt="profile" />
							<p>
								is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been
								the industry's standard dummy text ever since the 1500s
							</p>
							<h5>Karmani</h5>
							<p>FOUNDER AND CEO OF KARMANI</p>
						</div>
					</div>
				</div>
				<div class="carousel-item" data-bs-interval="2000">
					<div class="slide-section">
						<div class="textSection">
							<img src={profile} alt="profile" />
							<p>
								is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been
								the industry's standard dummy text ever since the 1500s
							</p>
							<h5>Karmani</h5>
							<p>FOUNDER AND CEO OF KARMANI</p>
						</div>
					</div>
				</div>
				<div class="carousel-item">
					<div class="slide-section">
						<div class="textSection">
							<img src={profile} alt="profile" />
							<p>
								is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been
								the industry's standard dummy text ever since the 1500s
							</p>
							<h5>Karmani</h5>
							<p>FOUNDER AND CEO OF KARMANI</p>
						</div>
					</div>
				</div>
			</div>
			<button
				class="carousel-control-prev"
				type="button"
				data-bs-target="#carouselExampleDark"
				data-bs-slide="prev"
			>
				<span class="carousel-control-prev-icon" aria-hidden="true" />
				<span class="visually-hidden">Previous</span>
			</button>
			<button
				class="carousel-control-next"
				type="button"
				data-bs-target="#carouselExampleDark"
				data-bs-slide="next"
			>
				<span class="carousel-control-next-icon" aria-hidden="true" />
				<span class="visually-hidden">Next</span>
			</button>
		</div>
	</div>
</section>

<style scoped lang="scss">
	@import './../../../assets/scss/variable';
	.testimonial-container {
		.left-background {
			position: absolute;
			background-color: #fff1ff;
			width: 650px;
			height: 200px;
		}
		.right-background {
			position: absolute;
			width: 171px;
			height: 157px;
			background-image: url(../../../assets/images/Frame.png);
			background-repeat: no-repeat;
			right: 0;
		}
		.slide-section {
			position: relative;
			width: 60%;
			height: auto;
			margin-left: 35%;
			padding: 60px 0px 10px 0px;
			text-align: center;
			.textSection {
				background-color: $white;
				box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.1);
				padding: 60px 10px 10px 10px;
				border-radius: 18px;
				&::after {
					content: '';
					position: absolute;
					background-image: url(../../../assets/images/comma_Left.png);
					background-repeat: no-repeat;
					background-size: contain;
					width: 25px;
					height: 19px;
					left: 30px;
					top: 90px;
				}
				&::before {
					content: '';
					position: absolute;
					background-image: url(../../../assets/images/comma_Right.png);
					background-repeat: no-repeat;
					background-size: contain;
					width: 25px;
					height: 19px;
					right: 30px;
					bottom: 30px;
				}
				img {
					position: absolute;
					top: 10px;
					margin: auto;
					left: 0;
					right: 0;
				}
				p {
					font-weight: 400;
					opacity: 0.5;
					font-size: 14px;
					padding-bottom: 20px;
					width: 77%;
					margin: auto;
				}
			}
		}
		.carousel-control-prev,
		.carousel-control-next {
			background-color: $primary;
			position: absolute;
			width: 100px;
			height: 70px;
			top: 160px;
			opacity: 1;
		}
		.carousel-control-prev {
			left: 30%;
			border-radius: 10px 0 0 10px;
		}
		.carousel-control-next {
			left: 36%;
			border-radius: 0 10px 10px 0;
		}
	}
</style>
