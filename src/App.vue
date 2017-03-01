<template>
  <div id="app">
    <img src="./assets/logo.png">
    <h1>{{msg}}</h1>
    <ul>
      <li v-for="a in staff">{{a.name}}</li>
    </ul>

  </div>
</template>

<script>
  export default {
    name: 'app',
    data () {
      return {
        msg: 'Go Karting Attendance List',
        attendees: [],
        staff: [
          { id: 1, name: 'Adam', branch: 'Swindon', attending: false },
          { id: 2, name: 'Paul', branch: 'Swindon', attending: true },
          { id: 3, name: 'Charlie', branch: 'Swindon', attending: true },
          { id: 4, name: 'Jodie', branch: 'Swindon', attending: true },
          { id: 5, name: 'Amber', branch: 'Swindon', attending: true },
          { id: 6, name: 'Peter', branch: 'Swindon', attending: false },
          { id: 7, name: 'Megan', branch: 'Swindon', attending: true },
          { id: 8, name: 'Alexa', branch: 'Bracknell', attending: false },
          { id: 9, name: 'Nicole', branch: 'Bracknell', attending: true },
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>
  $primary: #ff00ff;

  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }

  h1, h2 {
    font-weight: normal;
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
    color: $primary;
  }
</style>
