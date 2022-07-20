<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      Junior Backend Developer
    </p>
    <h3>Contact me</h3>
    <ul>
      <li>rachid.oulgour83@gmail.com</li>
      <!-- <li>628943543</li> -->
    </ul>
    <h3>Social Media</h3>
    <template>
        <vs-button flat @click="active=!active">
          {{ active ? 'Contact me' : 'Contact' }}
        </vs-button>

        <vs-alert closable v-model="active">
    <template #title>
        Email
    </template>
      <ul>
        <li>rachid.oulgour83@gmail.com</li>
      <!-- <li>628943543</li> -->
      </ul>
    </vs-alert>
  </template>

    <ul>
      <li><a href="https://www.linkedin.com/in/rachid-oulgour-870a1964/" target="_blank" rel="noopener">LinkedIn</a></li>
      <li><a href="https://github.com/Rachidoulgour" target="_blank" rel="noopener">GitHub</a></li>
      <!-- <li><a href="https://chat.vuejs.org" target="_blank" rel="noopener">Community Chat</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank" rel="noopener">Twitter</a></li>
      <li><a href="https://news.vuejs.org" target="_blank" rel="noopener">News</a></li> -->
    </ul>
    <!-- <h3>Ecosystem</h3>
    <ul>
      <li><a href="https://router.vuejs.org" target="_blank" rel="noopener">vue-router</a></li>
      <li><a href="https://vuex.vuejs.org" target="_blank" rel="noopener">vuex</a></li>
      <li><a href="https://github.com/vuejs/vue-devtools#vue-devtools" target="_blank" rel="noopener">vue-devtools</a></li>
      <li><a href="https://vue-loader.vuejs.org" target="_blank" rel="noopener">vue-loader</a></li>
      <li><a href="https://github.com/vuejs/awesome-vue" target="_blank" rel="noopener">awesome-vue</a></li>
    </ul> -->
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data:() => ({
        active: false,
      })
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
