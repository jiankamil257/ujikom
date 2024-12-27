<template>
  <div class="row bg-primary text-white align-items-center">
    <div class="col-lg-1 d-flex justify-content-center">
      <img src="../asset/img/Logo_SMK_Negeri_4_Tasikmalaya.png" alt="logo SMKN 4" width="80">
    </div>
    <div class="col-lg-8">
      <h1>Website Sekolah</h1>
      <address>
        SMKN 4 Tasikmalaya<br />
        Jl. Depok, Sukamenak, Purbaratu
      </address>
    </div>
    <div class="col-lg-3 d-flex justify-content-end">
      <ul class="navbar-nav d-flex flex-row align-items-center">
        <li class="nav-item mx-2">
          <a class="nav-link active" aria-current="page" href="#">Home</a>
        </li>
        <li class="nav-item mx-2">
          <a class="nav-link" href="/kontak">kontak</a>
        </li>
        <li class="nav-item mx-2">
          <a class="nav-link" href="/jurusan">jurusan</a>
        </li>
        <li class="nav-item mx-2">
          <a class="nav-link disabled">Disabled</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
.nav-link {
  color: #fff;
  text-decoration: none;
  transition: color 0.3s ease;
}

.nav-link:hover {
  color: #ccc;
}

.nav-link.disabled {
  color: #aaa;
  pointer-events: none;
}

h1 {
  font-size: 1.8rem;
  margin-bottom: 0;
}

address {
  font-style: normal;
  margin: 0;
  line-height: 1.5;
}
</style>
