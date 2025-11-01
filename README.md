<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>IPAL MBG - Bio Prima</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header class="hero">
    <div class="overlay"></div>
    <div class="hero-content">
      <h1>IPAL MBG</h1>
      <p>Solusi Pengolahan Limbah Ramah Lingkungan & Sesuai Standar DLH</p>
      <a href="#produk" class="btn-primary">Lihat Produk</a>
    </div>
  </header>

  <section id="tentang" class="section about">
    <h2>Tentang Kami</h2>
    <p><strong>CV Prima Mahardika (BIOPRIMA)</strong> adalah perusahaan berpengalaman dalam perencanaan, pembuatan, instalasi, dan perawatan IPAL. Kami berkomitmen menyediakan sistem IPAL berkualitas tinggi sesuai standar nasional dan internasional.</p>
    <div class="cert">
      <span>✅ Tersertifikasi ISO</span>
      <span>✅ Terdaftar di LPSE</span>
      <span>✅ Sesuai Standar DLH</span>
    </div>
  </section>

  <section id="produk" class="section produk">
    <h2>Produk & Program IPAL MBG</h2>
    <div class="produk-container">
      <div class="card">
        <img src="img/iklan-ipal-mbg-2025.jpg" alt="IPAL MBG">
        <h3>IPAL Paket Lengkap MBG</h3>
        <p>Menyediakan paket IPAL sesuai standar mutu dan ketentuan pemerintah. Cocok untuk program MBG dan kebutuhan dapur industri.</p>
      </div>

      <div class="card">
        <img src="img/gambar-iklan-ipal-slide-5.jpg" alt="IPAL Dapur MBG">
        <h3>IPAL Dapur Modular</h3>
        <p>Desain modular, efisien biaya, mengurangi bau & lemak saluran. Memenuhi standar DLH & peraturan pemerintah.</p>
      </div>

      <div class="card">
        <img src="img/iklan-ipal-gama-2.jpg" alt="Bio Prima IPAL">
        <h3>BioPrima IPAL</h3>
        <p>Sistem IPAL berkualitas tinggi, dirancang untuk efisiensi energi dan kemudahan perawatan jangka panjang.</p>
      </div>
    </div>
  </section>

  <section class="section kontak">
    <h2>Hubungi Kami</h2>
    <p>📍 Puri Kartika Asri, Malang<br>📞 0899-717-3518</p>
    <a href="https://wa.me/628997173518" target="_blank" class="btn-whatsapp">Chat via WhatsApp</a>
  </section>

  <footer>
    <p>© 2025 CV Prima Mahardika (BioPrima) | Semua Hak Dilindungi</p>
  </footer>

  <script>                 
    // Load data dari JSON
    fetch("data.json")
      .then(res => res.json())
      .then(data => {
        console.log("Data produk:", data);
      });
  </script>
</body>
</html>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
}

body {
  color: #333;
  background-color: #f8fafc;
  line-height: 1.6;
}

.hero {
  position: relative;
  background: url('img/iklan-ipal-gama-2.jpg') center/cover no-repeat;
  height: 90vh;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  text-align: center;
}

.overlay {
  position: absolute;
  top: 0; left: 0;
  width: 100%; height: 100%;
  background: rgba(0, 60, 30, 0.6);
}

.hero-content {
  position: relative;
  z-index: 2;
}

.btn-primary {
  background: #00b894;
  color: white;
  padding: 10px 25px;
  border-radius: 25px;
  text-decoration: none;
  transition: 0.3s;
}

.btn-primary:hover {
  background: #019875;
}

.section {
  padding: 60px 20px;
  text-align: center;
}

.about p {
  max-width: 700px;
  margin: 20px auto;
}

.cert {
  display: flex;
  justify-content: center;
  gap: 15px;
  margin-top: 15px;
  flex-wrap: wrap;
}

.produk-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 30px;
  margin-top: 30px;
}

.card {
  background: white;
  border-radius: 12px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
  width: 300px;
  transition: 0.3s;
}

.card:hover {
  transform: translateY(-5px);
}

.card img {
  width: 100%;
  border-radius: 12px 12px 0 0;
}

.card h3 {
  margin: 15px 0 5px;
  color: #006b4f;
}

.card p {
  padding: 0 15px 20px;
  font-size: 0.95em;
}

.kontak {
  background: #004d40;
  color: white;
}

.btn-whatsapp {
  background: #25D366;
  color: white;
  padding: 10px 25px;
  border-radius: 25px;
  text-decoration: none;
  display: inline-block;
  margin-top: 15px;
}

footer {
  background: #002b23;
  color: white;
  text-align: center;
  padding: 15px;
  font-size: 0.9em;
}

                                                            
