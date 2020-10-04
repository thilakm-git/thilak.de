<template>
	<div class="author">
		<g-image alt="Thilak Mahendran" class="author__image" src="~/assets/images/author.jpg" width="3667" height="1600"/>

		<h1>Thilak Mahendran</h1>
		<p>Head of <a href="https://www.bva.bund.de/DE/Services/Behoerden/Beratung/Beratungszentrum/OpenData/opendata_node.html">Open Data<svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" x="0px" y="0px" viewBox="0 0 100 100" width="15" height="15" class="icon outbound"><path fill="currentColor" d="M18.8,85.1h56l0,0c2.2,0,4-1.8,4-4v-32h-8v28h-48v-48h28v-8h-32l0,0c-2.2,0-4,1.8-4,4v56C14.8,83.3,16.6,85.1,18.8,85.1z"></path> <polygon fill="currentColor" points="45.7,48.7 51.3,54.3 77.2,28.5 77.2,37.2 85.2,37.2 85.2,14.9 62.8,14.9 62.8,22.9 71.5,22.9"></polygon></svg></a> at the Federal Office of Administration of the German Government</p>

		<p class="author__links">
		<a href="//twitter.com/thilakmahendran"><font-awesome :icon="['fab', 'twitter']"/></a>
		<a href="//linkedin.com/in/thilakmahendran"><font-awesome :icon="['fab', 'linkedin-in']"/></a>
		<a href="//github.com/thilakm-git"><font-awesome :icon="['fab', 'github']"/></a>
		<a href="/blog"><font-awesome :icon="['far', 'bookmark']"/></a>
		</p>

	</div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
export default {
	props: ['showTitle']
}
</script>

<style lang="scss">
.author {
	margin: 0 auto;
	max-width: 600px;
	text-align: center;
	padding: calc(var(--space) / 2) 0;

	&__image {
		object-fit: contain;
		margin-bottom: 1em;
	}

	&__intro {
		opacity: .8;
	}

	&__site-title {
		font-size: 1.5em;
	}

	&__links {
		margin-top: -.5em;
		a {
			margin: 0 .5em;
		}
	}
}
</style>