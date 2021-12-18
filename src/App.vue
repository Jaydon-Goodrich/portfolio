<template>
	<div id="app" style="background-color: #0d0d0d;">
		<Profile />
	</div>
</template>

<script>
	import Profile from './components/Profile.vue'

	export default {
		name: 'App',
		components: {
			Profile
		}
	}
</script>

<style>
	html {
		overflow: hidden;
		height: 100%;
	}

	body {
		overflow: auto;
		height: 100%;
	}
</style>
