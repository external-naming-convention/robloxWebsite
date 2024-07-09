<template>
	<div class="section footer">
		<div class="content">
			<img src="@/assets/ENC-Supported.png" alt="" />
			<sub>A collaboration to provide better scripting!</sub>
			<p v-if="$route.path != '/badge'">
				Have <em>you</em> added RENC support already? <router-link to="/badge">Feature the RENC badge on your website</router-link>!
			</p>
		</div>
		<div class="aside">
			<p class="opensource">
				This website is open source on <a href="https://github.com/external-naming-convention/robloxWebsite" target="_blank">GitHub</a>.
			</p>
		</div>
	</div>
</template>

<style lang="scss" scoped>
.section {
	display: grid;
	grid-template-columns: 1fr 1fr;
	gap: 20%;
	.content {
		display: flex;
		flex-direction: column;
		align-items: left;
		img {
			width: 120px;
			margin-bottom: 0.5rem;
		}

		sub {
			font-style: italic;
			color: $text-secondary;
			margin-bottom: 1rem;
		}

		p {
			font-size: 1.2rem;
			line-height: 1.5;

			em {
				text-decoration: underline;
			}

			a {
				color: lighten($secondary, 10%);
				text-decoration: none;
			}
		}
	}
	.aside {
		text-align: right;
		p {
			font-size: 1.5rem;
			line-height: 1.5;
			color: $text-secondary;
			a {
				color: lighten($secondary, 10%);
				text-decoration: none;
			}

			&.opensource {
				font-size: 1.25rem;
			}
		}

		.footnotes {
			margin-top: 1rem;
			p {
				color: $text-secondary;
				font-size: 1.2rem;
			}
		}
	}
}
</style>
