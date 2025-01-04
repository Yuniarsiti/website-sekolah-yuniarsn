<template>
  <div class="container">
    <div class="profile">
      <img class="photo" :src="photo" alt="Profile Picture" />
      <div class="info">
        <h1>{{ name }}</h1>
        <p><strong>Hobi:</strong> {{ hobby }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Biodata',
  data() {
    return {
      name: 'Yuniar Siti Nurhaliza',
      hobby: 'Mendengarkan musik, Menonton',
      photo: 'https://drive.google.com/file/d/1gtOSdNZEYcoLbE34H619wTiUIVqGzDM8/View?usp=drivedsk', // Ganti dengan URL foto kamu
    };
  },
};
</script>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.profile {
  display: flex;
  align-items: center;
  background-color: #f4f4f4;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.photo {
  width: 200px; /* Lebar foto */
  height: 200px; /* Tinggi foto */
  object-fit: cover; /* Menjaga proporsi foto */
  margin-right: 20px;
}

.info h1 {
  font-size: 24px;
  margin: 0;
}

.info p {
  font-size: 18px;
  margin-top: 8px;
}
</style>
