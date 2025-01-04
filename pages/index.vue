<template>
  <div class="container-fluid p-0">
    <section class="hero">
      <div class="content">
        <h4>Selamat Datang di Website Resmi</h4>
        <h1 class="fw-semibold">SMKN 4 Tasikmalaya</h1>
      </div>
    </section>
  
    <!-- Seksi Visi -->
    <section class="info">
      <div class="container">
        <h3 class="text-center">Visi Sekolah</h3>
        <p class="mt-3 text-center">Terwujudnya lulusan yang Cerdas, Aktif, Kompetitif, Adaptif dan Produktif berlandaskan Iman dan Takwa (CAKAP BERIMTAK)</p>
  
        <!-- <h3>Sejarah Singkat</h3> -->
        <!-- <p>SMKN 4 Tasikmalaya berdiri sejak tahun 2010 </p> -->
      </div>
    </section>

    <!--Seksi Sambutan-->
    <div class="sambutan">
      <h3 class="text-center">Sambutan Kepala Sekolah</h3>
      <div class="row justify-content-center">
        <div class="col-md-4">
          <img src="../assets/kepsekk.png" alt="kepsekk">
        </div>
        <div class="col-md-8">
          <h4 class="mt-4">Kurniawan S.Pd, M.Pd</h4>
          <h6 class="mt-4">Assalamualaikum Warahmatullahi Wabarakatuh</h6>
          <h6 class="mt-4">Segala puji dan syukur kita panjatkan kehadirat Allah SWT, semoga kita semua ada dalam lindungan-Nya. Dan atas perkenan-Nya pula kami dapat menghadirkan website SMK Negeri 4 Tasikmalaya ini. Kami berharap dengan adanya website di SMK Negeri 4 Tasikmalaya ini para pengunjung dapat mengenal lebih jauh tentang sekolah kami sehingga dapat mempererat tali silaturrahmi antara sekolah dengan masyarakat demi kemajuan kita bersama. Tiada gading yang tak retak, website kami ini masih dalam proses pengembangan, masih banyak kekurangan yang harus kami perbaiki. Kritik dan sarannya yang membangun sangat kami harapkan untuk pengembangan ke depan.</h6>
          <h6 class="mt-4">Akhirnya, saya mengucapkan terimakasih yang sebesar-besarnya kepada semua pihak yang tidak dapat disebutkan satu segala bantuan dan persatu atas fasilitasnya yang telah diberikan semoga semua yang kita lakukan bermanfaat bagi masyarakat.</h6>
          <h6 class="mt-4">Wassalamu'alaikum Warahmatullahi Wabarakatuh.</h6>
        </div>
      </div>
    </div>
  
    <!-- Seksi Jurusan -->
    <section class="departments mb-5">
      <div class="container">
        <h3 class="text-center">Konsentrasi Keahlian</h3>
        <div class="department-list mt-3">
          <!-- Jurusan 1 -->
          <div class="department">
            <img src="~/assets/tkjt.png" alt="Teknik jaringan komputer" class="department-logo"/>
            <h3>Teknik Komputer dan Jaringan</h3>
          </div>
          <!-- Jurusan 2 -->
          <div class="department">
            <img src="~/assets/pplg.png" alt="Pengembangan Perangkat Lunak Gim" class="department-logo"/>
            <h3>Pengembangan Perangkat Lunak Gim</h3>
          </div>
          <!-- Jurusan 3 -->
          <div class="department">
            <img src="~/assets/tbsm.png" alt="Teknik Sepeda Motor" class="department-logo"/>
            <h3>Teknik Sepeda Motor</h3>
          </div>
          <!-- Jurusan 4 -->
          <div class="department">
            <img src="~/assets/toi.png" alt="Teknik Otomasi Industri" class="department-logo"/>
            <h3>Teknik Otomasi Industri</h3>
          </div>
          <!-- Jurusan 5 -->
          <div class="department">
            <img src="~/assets/dkv.png" alt="Desain Komunikasi Visual" class="department-logo"/>
            <h3>Desain Komunikasi Visual</h3>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<style scoped>
.hero {
  background-image: url('~/assets/smkn44.jpg');
  background-size: cover;
  background-position: center;
  height: 80vh;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #ebebf4;
  text-align: center;
}

.info {
  background-color: #f8f8f8;
  padding: 30px;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
}

h2, h3 {
  color: #0E0E55;
}

p {
  font-size: 1.3rem;
  line-height: 1.6;
  color: #150e0e;
}

/* Styling untuk bagian jurusan */
.departments {
  background-color: #f0f0f0;
  padding: 50px 0;
}

.department-list {
  display: grid;
  grid-template-columns: repeat(3, 1fr); /* 3 kolom untuk bagian atas */
  gap: 20px;
  margin-bottom: 20px;
}

.department-list > .department:nth-child(4),
.department-list > .department:nth-child(5) {
  grid-column: span 1; /* Membuat jurusan ke-4 dan ke-5 berdampingan */
}

.department {
  text-align: center;
  background-color: #fff7f7;
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.department-logo {
  width: 100px;
  height: 100px;
  object-fit: cover;
  border-radius: 50%;
  margin-bottom: 15px;
}

.department h3 {
  color: #0E0E55;
  font-size: 1.2rem;
}

.department p {
  font-size: 1rem;
  color: #777;
}

.sambutan {
  padding: 30px;
}

.sambutan h4, .sambutan h6 {
  margin-left: 30px;
}
</style>