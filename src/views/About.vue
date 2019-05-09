<template>
  <div class="about">
    <router-link to="/">Navigate to Home</router-link>
    <p>Screen About</p>
    <p>Watch the title and the url, they are programmatically set</p>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'home',
  mounted () {
    history.pushState('', '', '/about_url_dynamically_set')
	document.title = 'About title programmatically set'
  }
}
</script>
