<template>
	<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
		<a class="navbar-brand" href="#">{{brand}}</a>
		<button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#mainNav" aria-controls="mainNav" aria-expanded="false" aria-label="Toggle navigation">
			<span class="navbar-toggler-icon"></span>
		</button>

		<div class="collapse navbar-collapse d-lg-flex justify-content-xl-center code2" id="mainNav">
			<ul class="navbar-nav">
				<li class="nav-item active" v-for="nav in navs">
					<a class="nav-link" :href="nav.href" :title="nav.title">{{nav.link}}</a>
				</li>
			</ul>
		</div>
	</nav>
</template>


<script>
	import 'bootstrap';
	export default {
		name: "Navbar",
		data() {
			return {
				brand: "",
				navs : [
					{
						link: "Home",
						href: "#"
					},
					{
						link: "About",
						href: "#"
					},
					{
						link: "My Work",
						href: "#",
						title: "Past, Present, and Pitches"
					},
					{
						link: "Contact",
						href: "#"
					}
				]
			}
		}
	}
</script>


<style lang="scss" scoped>

</style>