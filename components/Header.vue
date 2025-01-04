<template>
  <div class="container-fluid p-0">
    <div class="header-school">
        <div class="row align-items-center m-0">
          <!-- Logo -->
          <div class="col-lg-2 col-md-3 col-4 text-center">
            <img src="~/assets/LOGO1.png" alt="LOGO1" class="logo m-3" />
          </div>
  
          <!-- Informasi Kontak -->
          <div class="col-lg-10 col-md-9 col-8">
            <div class="contact-info">
              <p>
                <i class="fas fa-map-marker-alt"></i> Jl. Depok, Sukamenak, Purbaratu, Tasikmalaya
              </p>
              <p>
                <i class="fas fa-phone-alt"></i> (0265) 123456
              </p>
              <p>
                <i class="fas fa-envelope"></i> info@smkn4tasik.sch.id
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <style scoped>
  @import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css');
  @import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;600&display=swap');
  
  /* Header Styling */
  .header-school {
    background-color: #0E0E55;
    color: white;
  }
  
  .logo {
    max-width: 60px;
  }
  
  /* Kontak Styling */
  .contact-info {
    font-family: "Open Sans", sans-serif;
    font-size: 0.9rem;
    display: flex;  /* Flexbox untuk tata letak horizontal */
    justify-content: flex-end; /* Menempatkan semua item ke kanan */
    align-items: center;
    gap: 30px; /* Jarak antar item */
    margin-right: 50px;
  }
  
  .contact-info p {
    margin: 0;
    display: flex;
    align-items: center;
    gap: 10px;
  }
  
  .contact-info i {
    color: #f0eee5; /* Warna ikon */
    font-size: 1.2rem;
  }
  </style>