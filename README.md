# Lab6Web.

Tugas Pemograman Web1 Pertemuan 6

    Nama: Burhan Isnain Nur Huda
    NIM: 312410226
    Kelas: TI.24.A.2
    Mata Kuliah: Pemograman Web1

## Praktikum 6: Web Framework — CryptoVerse

## Tujuan Praktikum

1. Mahasiswa memahami konsep dasar Web Framework.
2. Mahasiswa memahami struktur layout web menggunakan CSS Framework (Bootstrap).
3. Mahasiswa mampu menerapkan elemen-elemen Bootstrap untuk membangun website responsif dan menarik.

   ## Langkah 1 — Persiapan Project
## Struktur Folder:
Lab6Web

1. index.html
2.  style.css
3.   script.js

 ## Penjelasan:

index.html → file utama untuk struktur dan konten website.

style.css → file CSS tambahan untuk mempercantik tampilan.

script.js → berisi logika untuk menampilkan grafik menggunakan Chart.js.

## Screenshot 1 — Struktur folder di VSCode
<img width="196" height="100" alt="image" src="https://github.com/user-attachments/assets/3e2a580e-87ce-4757-80fb-81215ccc8420" />

## Langkah 2 — Membuat File index.html

File ``index.html`` berisi struktur utama website menggunakan Bootstrap 5.3.3 dan Chart.js.

## Kode:

    <!DOCTYPE html>
    <html lang="id">
    <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CryptoVerse - Praktikum 6 Web Framework</title>
  <!-- Bootstrap -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <!-- Chart.js -->
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
  <!-- Custom CSS -->
    <link rel="stylesheet" href="style.css">
    </head>

    <body class="bg-dark text-light">

  <!-- Navbar -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-secondary shadow-sm">
    <div class="container">
      <a class="navbar-brand fw-bold text-info" href="#">💰 CryptoVerse</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link" href="#">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Trending</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Tips</a></li>
          <li class="nav-item"><a class="nav-link" href="#">About</a></li>
        </ul>
      </div>
    </div>
     </nav>

  <!-- Container Utama -->
    <div class="container my-5">
    <div class="row g-4">
      
      <!-- Trending Coins -->
      <div class="col-md-4">
        <div class="card bg-secondary p-3 shadow-lg">
          <h4 class="text-info mb-3">🔥 Trending Coins</h4>
          <ul class="list-group list-group-flush">
            <li class="list-group-item bg-transparent text-white">1. Bitcoin (BTC) <span class="text-success fw-bold">$115,548.60</span></li>
            <li class="list-group-item bg-transparent text-white">2. Ethereum (ETH) <span class="text-success fw-bold">$4,229.73</span></li>
            <li class="list-group-item bg-transparent text-white">3. Binance Coin (BNB) <span class="text-success fw-bold">$1,153.23</span></li>
            <li class="list-group-item bg-transparent text-white">4. Ripple (XRP) <span class="text-success fw-bold">$2.71</span></li>
            <li class="list-group-item bg-transparent text-white">5. Solana (SOL) <span class="text-success fw-bold">$209.61</span></li>
            <li class="list-group-item bg-transparent text-white">6. Dogecoin (DOGE) <span class="text-success fw-bold">$0.2161</span></li>
            <li class="list-group-item bg-transparent text-white">7. TRON (TRX) <span class="text-success fw-bold">$0.3412</span></li>
            <li class="list-group-item bg-transparent text-white">8. Cardano (ADA) <span class="text-success fw-bold">$0.6972</span></li>
            <li class="list-group-item bg-transparent text-white">9. Hype (HYPE) <span class="text-success fw-bold">$49.19</span></li>
          </ul>
        </div>

        <!-- Crypto Tips -->
        <div class="card bg-secondary mt-4 p-3 shadow-lg">
          <h4 class="text-warning mb-3">💡 Crypto Tips</h4>
          <ul class="list-group list-group-flush text-white">
            <li class="list-group-item bg-transparent">1️⃣ <b>DCA (Dollar Cost Averaging):</b> Investasi rutin tiap minggu/bulan tanpa peduli harga naik-turun.</li>
            <li class="list-group-item bg-transparent">2️⃣ <b>FOMO:</b> Hindari beli karena ikut-ikutan tren, bisa nyangkut di harga puncak.</li>
            <li class="list-group-item bg-transparent">3️⃣ <b>DYOR:</b> Lakukan riset sendiri sebelum membeli aset baru.</li>
            <li class="list-group-item bg-transparent">4️⃣ <b>HODL:</b> Tahan aset berkualitas saat pasar turun, jangan panik.</li>
            <li class="list-group-item bg-transparent">5️⃣ <b>Diversifikasi:</b> Jangan taruh semua modal di satu koin, sebar risiko.</li>
          </ul>
        </div>
      </div>

      <!-- Apa itu Cryptocurrency -->
      <div class="col-md-8">
        <div class="card bg-secondary p-4 shadow-lg">
          <h3 class="text-info mb-3">🚀 Apa itu Cryptocurrency?</h3>
          <p class="text-white">
            Cryptocurrency adalah bentuk mata uang digital yang menggunakan teknologi blockchain untuk memastikan keamanan dan transparansi setiap transaksi. Nilainya sangat dinamis dan bisa berubah karena faktor makroekonomi seperti inflasi global, pergerakan nilai dolar, kebijakan bank sentral, hingga kondisi geopolitik.
          </p>
          <p class="text-white">
            Selain itu, faktor mikroekonomi seperti adopsi pengguna, kepercayaan komunitas, inovasi teknologi, serta perkembangan ekosistem tiap proyek juga berperan besar dalam menentukan nilai pasar crypto.
          </p>
          <button class="btn btn-primary mt-2">Pelajari Lebih Lanjut</button>
        </div>

        <!-- Grafik Bitcoin dan Ethereum -->
        <div class="row mt-4">
          <div class="col-md-6">
            <div class="card bg-secondary p-3 shadow-lg">
              <h5 class="text-info">📈 Bitcoin (BTC)</h5>
              <p class="text-success fw-bold">$115,548.60</p>
              <p class="text-muted">Total Market Cap: $2.1 Triliun</p>
              <canvas id="btcChart"></canvas>
            </div>
          </div>
          <div class="col-md-6">
            <div class="card bg-secondary p-3 shadow-lg">
              <h5 class="text-info">🪙 Ethereum (ETH)</h5>
              <p class="text-success fw-bold">$4,229.73</p>
              <p class="text-muted">Total Market Cap: $700 Miliar</p>
              <canvas id="ethChart"></canvas>
            </div>
          </div>
        </div>
      </div>
    </div>
    </div>

  <!-- Footer -->
    <footer class="text-center py-3 mt-5 bg-secondary text-light">
    <small>© 2025 CryptoVerse | Dibuat untuk Praktikum Web Framework</small>
    </footer>

  <!-- Script -->
    <script src="script.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>

    </body>
    </html>

## Screenshot 2 — Tampilan awal website di browser
<img width="1903" height="894" alt="image" src="https://github.com/user-attachments/assets/41ae6536-623f-42aa-a4cb-108ebaee970d" />

## Langkah 3 — File style.css

## Kode:

    body {
    background-color: #0d1117;
    }

    .card {
    border-radius: 15px;
    border: 1px solid #30363d;
    }

    .text-info {
    color: #00bfff !important;
    }

    .text-success {
    color: #00ff87 !important;
    }

    .btn-primary {
    background: linear-gradient(90deg, #007bff, #0066ff);
    border: none;
    font-weight: 600;
    }

    .btn-primary:hover {
    background: linear-gradient(90deg, #0066ff, #004de6);
    }

## Penjelasan:

1. Warna utama gelap (#0d1117) untuk nuansa crypto modern.

2. Card dan tombol diberi efek gradient agar tidak monoton.

3. Warna teks diatur agar kontras dan nyaman dibaca di dark mode.

## Screenshot 3 — Tampilan card dan button setelah styling
<img width="1919" height="896" alt="image" src="https://github.com/user-attachments/assets/baf28819-6026-4ab4-8b5b-2c29026d83d3" />

## Langkah 4 — File script.js

## Kode:

    // Grafik BTC
    const ctxBTC = document.getElementById('btcChart').getContext('2d');
    new Chart(ctxBTC, {
    type: 'line',
     data: {
    labels: ['Jan', 'Feb', 'Mar', 'Apr', 'Mei', 'Jun', 'Jul'],
    datasets: [{
      label: 'BTC Price',
      data: [95000, 100000, 110000, 120000, 118000, 115000, 115548],
      borderColor: '#ff9900',
      borderWidth: 2,
      fill: false
    }]
    },
    options: { scales: { y: { beginAtZero: false } } }
    });

    // Grafik ETH
    const ctxETH = document.getElementById('ethChart').getContext('2d');
    new Chart(ctxETH, {
    type: 'line',
    data: {
    labels: ['Jan', 'Feb', 'Mar', 'Apr', 'Mei', 'Jun', 'Jul'],
    datasets: [{
      label: 'ETH Price',
      data: [3500, 3700, 4000, 4300, 4200, 4100, 4229],
      borderColor: '#00bfff',
      borderWidth: 2,
      fill: false
    }]
    },
    options: { scales: { y: { beginAtZero: false } } }
    });

## Penjelasan:

1. Menggunakan Chart.js untuk menampilkan grafik harga BTC dan ETH.

2. Data disimulasikan berdasarkan pergerakan harga bulanan.

3. Warna grafik disesuaikan dengan tema crypto: oranye untuk BTC dan biru untuk ETH.

## Screenshot 4 — Tampilan grafik BTC dan ETH
<img width="1917" height="900" alt="image" src="https://github.com/user-attachments/assets/3cb0c782-2eec-4a21-b943-578cda210528" />


