<template>
  <div id="app">
    <header class="bg-dark py-3">
      <nav class="navbar navbar-expand-lg bg-body-tertiary">
        <div class="container-fluid">
          <a class="navbar-brand" href="#">Widget Adelia</a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarNavDropdown">
            <ul class="navbar-nav">
              <li class="nav-item">
                <a class="nav-link active" aria-current="page" href="/Home.vue">Home</a>
              </li>
              <li class="nav-item">
                <router-link to="/cuaca" class="nav-link"
                  >Cuaca</router-link>
              </li>
              <li class="nav-item">
                <router-link to="/location" class="nav-link"
                  >Lokasi</router-link>
              </li>
              <li class="nav-item">
                <router-link to="/stopwatch" class="nav-link"
                  >Stopwatch</router-link>
              </li>
              <li class="nav-item">
                <router-link to="/tictactoe" class="nav-link"
                  >Game</router-link>
              </li>
              <li class="nav-item">
                <router-link to="/photo" class="nav-link"
                  >Foto</router-link>
              </li>
            </ul>
          </div>
        </div>
      </nav>
    </header>
    <div class="container py-4">
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
import $ from "jquery";
export default {
  name: "App",
  mounted() {
    // Inisialisasi Navbar Toggler
    $(".navbar-toggler").on("click", function () {
      $(this).toggleClass("active");
    });
  },
};
</script>

<style>
#app {
  text-align: center;
}

header {
  background: #333;
  padding: 20px;
}

.navbar-brand {
  font-size: 24px;
}

.navbar-toggler {
  border: none;
  outline: none;
}

.nav-item {
  margin-right: 10px;
}

.nav-link {
  color: #fff;
  text-decoration: none;
  padding: 5px 10px;
  transition: color 0.3s;
}

.nav-link:hover {
  color: #aaa;
}

.container {
  max-width: 960px;
  margin: 0 auto;
}

.py-4 {
  padding-top: 2rem;
  padding-bottom: 2rem;
}
</style>npm
