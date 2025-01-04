<template>
  <div class="container-fluid p-0">
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
      <div class="container-fluid">
        
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav">
            <li class="nav-item">
              <nuxt-link to="/" class="nav-link active">Beranda</nuxt-link>
            </li>
            <li class="nav-item">
              <nuxt-link to="/profil" class="nav-link">Profil</nuxt-link>
            </li>
            <li class="nav-item">
              <nuxt-link to="/galeri" class="nav-link">Galeri</nuxt-link>
            </li>
            <li class="nav-item">
              <nuxt-link to="/ekstrakulikuler/" class="nav-link">Ekstrakurikuler</nuxt-link>
            </li>
            <li class="nav-item">
              <nuxt-link to="/berita/" class="nav-link">Berita</nuxt-link>
            </li>
            <li class="nav-item">
              <nuxt-link to="/biodata/" class="nav-link">Biodata</nuxt-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </div>
</template>

<style scoped>
.navbar {
  background-color: #eaeaf2;
}

.navbar-menu {
  display: flex;
  justify-content: center;
  list-style: none;
}

.navbar-menu li {
  margin: 0 15px;
}

.nav-link {
  color: rgb#0E0E55;
  text-decoration: none;
  font-size: 15px;
  font-family: 'Open Sans', sans-serif;
}

.nav-link:hover {
  color: #FFCC00; /* Ubah warna saat hover */
}
</style>