<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
     Welcome to the FridgiGo App! We are happy to see you!
    </p>
    <p>Please log in or sign up to use our app</p>
    <div v-if="!isAuthenticated"><button @click="login">Login or Sign up</button></div>
    <div v-else><button @click="logout">Logout</button></div>
  </div>
</template>

<script>
import Vue from 'vue'

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  computed: {
    isAuthenticated: () => {
      return Vue.$keycloak.authenticated
    }
  },
  methods: {
    login () {
      Vue.$keycloak.login({ redirectUri: window.location.origin })
    },
    logout () {
      Vue.$keycloak.logout({ redirectUri: window.location.origin })
    }
  }
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
p{
  background-color:#b2edef
}
template{
  background-color:#b2edef
}
</style>
