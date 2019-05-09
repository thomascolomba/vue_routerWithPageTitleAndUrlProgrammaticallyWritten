<template>
  <div class="home">
    <router-link to="/about">Navigate to About</router-link>
    <p>Screen Home</p>
    <p>Watch the title and the url, they are programmatically set</p>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'home',
  mounted () {
    history.pushState('', '', '/home_url_dynamically_set')
	document.title = 'Home title programmatically set'
  }
}
</script>
