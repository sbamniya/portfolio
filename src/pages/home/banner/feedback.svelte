<div class="feedback-box">
	<div class="feedback">
		<div class="image-container">
			<img src="/banner-image.png" alt="" class="client-image" />
		</div>
		<div class="meta-details">
			<div class="name">Phanny - Nigeria</div>
			<div class="date">Sat 28 May 2022</div>
		</div>
	</div>
	<p class="feeback-text">
		In just a few short years, I built the brand to millions of social media followers and websites
		visitors.
	</p>
</div>

<style scoped lang="scss">
	@import './../../../assets/scss/variable';
	@import './../../../assets/scss/mixins';

	.feedback-box {
		position: absolute;
		bottom: 0;
		background: $white;
		box-shadow: 0px 2.72153px 34.0191px rgba(19, 23, 61, 0.1);
		border-radius: 6.80382px;
		width: 375px;
		padding: 12px;
		display: flex;
		flex-wrap: wrap;
		row-gap: 12px;
		@include mq(sm) {
			position: static;
			width: 100%;
			margin-top: 20px;
		}

		.feedback {
			display: flex;
			align-items: center;
			column-gap: 10px;
			.image-container {
				.client-image {
					width: 40px;
					height: 40px;
					overflow: hidden;
					border-radius: 100px;
				}
			}
			.meta-details {
				font-family: $poppins-regular;
				.name {
					color: $black;
					font-size: $font-12;
				}
				.date {
					color: rgba($color: $black, $alpha: 0.5);
					font-size: $font-12;
				}
			}
		}

		.feeback-text {
			font-family: $poppins-regular;
			font-style: normal;
			font-weight: 400;
			font-size: $font-12;
			line-height: 20px;
			color: rgba($color: $black, $alpha: 0.7);
			margin-bottom: 0;
		}
	}
</style>
