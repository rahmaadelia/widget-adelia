<template>
  <div class="container">
    <center>
      <button type="button" class="btn btn-primary">Primary</button>

      <ul class="btn btn-primary">
              <li class="btn btn-primary">
                <router-link to="/cuaca" class="nav-link"
                  >Cuaca</router-link>
              </li>
              <li class="btn btn-primary">
                <router-link to="/location" class="nav-link"
                  >Lokasi</router-link>
              </li>
              <li class="btn btn-primary">
                <router-link to="/stopwatch" class="nav-link"
                  >Stopwatch</router-link>
              </li>
              <li class="btn btn-primary">
                <router-link to="/tictactoe" class="nav-link"
                  >Game</router-link>
              </li>
              <li class="btn btn-primary">
                <router-link to="/photo" class="nav-link"
                  >Foto</router-link>
              </li>
            </ul>
    </center>
  </div>
   
</template>

<script>
export default {
  name: 'Home',
  props: {
    msg: String
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
</style>
