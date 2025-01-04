<template>
  <div class="gallery-page">
    <header>
      <p>Galeri sekolah</p>
    </header>
    <section class="gallery-grid">
      <div
        v-for="photo in photos"
        :key="photo.id"
        class="gallery-item"
      >
        <img :src="photo.src" :alt="photo.alt" class="gallery-photo" />
        <p class="photo-caption">{{ photo.caption }}</p>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "GaleriPage",
  data() {
    return {
      photos: [
        {
          id: 1,
          src: "https://radartasik.id/wp-content/uploads/2023/03/Expo-Creanova-1.jpg",
          alt: "kegiatan expo",
          caption: "KEGIATAN EXPO",
        },
        {
          id: 2,
          src: "https://radartasik.id/wp-content/uploads/2023/04/LKS-RPL.jpg",
          alt: "LKS",
          caption: "LKS",
        },
        {
          id: 3,
          src: "https://radarcirebon.disway.id/upload/50ad6c4b064bae55698ffb74f6113df7.jpg",
          alt: "Kegiatan 3",
          caption: "Kegiatan Pramuka",
        },
        {
          id: 4,
          src: "https://radartasik.id/wp-content/uploads/2024/05/Duta-Safety-Riding-SMKN-4-Tasikmalaya-.webp",
          alt: "Kegiatan 4",
          caption: "Pentas Seni",
        },
        {
          id: 5,
          src: "https://ruangatas.com/wp-content/uploads/2023/10/Picsart_23-10-12_16-15-19-734-scaled.jpg",
          alt: "Kegiatan 5",
          caption: "Job fair",
        },
        {
          id: 6,
          src: "https://assets.radartasik.id/main/2024/10/SMKN-4-tasikmalaya-raih-beasiswa-AHM.webp",
          alt: "Kegiatan 6",
          caption: "Tujuh siswa smkn4 raih beasiswa dari astra honda motor",
        },
        {
          id: 7,
          src: "https://i.ytimg.com/vi/yHe3_0xv6yM/maxresdefault.jpg?sqp=-oaymwEmCIAKENAF8quKqQMa8AEB-AH-CYAC0AWKAgwIABABGGUgYChQMA8=&rs=AOn4CLCzVCL_eCveZVyzSpHCqs3bak8rHA",
          alt: "kegiatan 7",
          caption: "cover,sekar gending",
        }
      ],
    };
  },
};
</script>

<style scoped>
.gallery-page {
  font-family: Arial, sans-serif;
  text-align: center;
  margin: 20px auto;
  max-width: 1200px;
}

header h1 {
  font-size: 2rem;
  margin-bottom: 20px;
  color: #333;
}

.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
  padding: 10px;
}

.gallery-item {
  position: relative;
  overflow: hidden;
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.gallery-photo {
  width: 100%;
  height: auto;
  display: block;
  transition: transform 0.3s;
}

.gallery-item:hover .gallery-photo {
  transform: scale(1.1);
}

.photo-caption {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background: rgba(0, 0, 0, 0.7);
  color: white;
  padding: 10px;
  font-size: 0.9rem;
  text-align: center;
  opacity: 0;
  transition: opacity 0.3s;
}

.gallery-item:hover .photo-caption {
  opacity: 1;
}
</style>