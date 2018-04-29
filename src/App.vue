<template>
  <div class="row-fluid" id="app">
  	<Navbar />
  </div>
</template>

<script>
import Navbar from './components/Navbar';
export default {
  name: 'app',
  components: {
		Navbar
  }
}
</script>

<style lang="scss">
	@import '../node_modules/bootstrap/dist/css/bootstrap.min.css';
	@import './assets/scss/mastyle.css';
</style>
