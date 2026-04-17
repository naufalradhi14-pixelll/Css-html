# Css-html
Codingan
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SMA Negeri Harapan | Official Website</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <nav>
            <div class="logo">SMA Harapan</div>
            <ul>
                <li><a href="#">Beranda</a></li>
                <li><a href="#">Tentang Kami</a></li>
                <li><a href="#">Akademik</a></li>
                <li><a href="#">Kontak</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero">
        <div class="hero-text">
            <h1>Membangun Generasi Cerdas & Berkarakter</h1>
            <p>Selamat datang di website resmi SMA Negeri Harapan. Tempat terbaik untuk mengukir masa depan.</p>
            <a href="#" class="btn">Selengkapnya</a>
        </div>
    </section>

    <section class="info">
        <div class="container">
            <div class="card">
                <h3>Kurikulum</h3>
                <p>Menggunakan Kurikulum Merdeka yang inovatif dan fleksibel.</p>
            </div>
            <div class="card">
                <h3>Fasilitas</h3>
                <p>Laboratorium modern, perpustakaan digital, dan lapangan olahraga.</p>
            </div>
            <div class="card">
                <h3>Ekstrakurikuler</h3>
                <p>Wadahi bakat siswa melalui lebih dari 15 klub minat dan bakat.</p>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 SMA Negeri Harapan. All Rights Reserved.</p>
    </footer>

</body>
</html>
/* Pengaturan Dasar */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

body {
    line-height: 1.6;
    color: #333;
}

/* Navigasi */
nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 5%;
    background: #2c3e50;
    color: #fff;
    position: sticky;
    top: 0;
    z-index: 1000;
}

.logo {
    font-size: 1.5rem;
    font-weight: bold;
}

nav ul {
    display: flex;
    list-style: none;
}

nav ul li {
    margin-left: 20px;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
    transition: 0.3s;
}

nav ul li a:hover {
    color: #3498db;
}

/* Hero Section */
.hero {
    height: 60vh;
    background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), 
                url('https://images.unsplash.com/photo-1523050853064-dbad350c7469?auto=format&fit=crop&w=1350&q=80');
    background-size: cover;
    background-position: center;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    color: #fff;
}

.hero-text h1 {
    font-size: 3rem;
    margin-bottom: 10px;
}

.btn {
    display: inline-block;
    margin-top: 20px;
    padding: 10px 25px;
    background: #3498db;
    color: #fff;
    text-decoration: none;
    border-radius: 5px;
}

/* Info Cards */
.container {
    display: flex;
    justify-content: space-around;
    padding: 50px 5%;
    background: #f4f4f4;
}

.card {
    background: #fff;
    padding: 20px;
    width: 30%;
    text-align: center;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}

.card h3 {
    margin-bottom: 10px;
    color: #2c3e50;
}

/* Footer */
footer {
    text-align: center;
    padding: 20px;
    background: #2c3e50;
    color: #fff;
}

/* Responsif untuk HP */
@media (max-width: 768px) {
    .container {
        flex-direction: column;
    }
    .card {
        width: 100%;
        margin-bottom: 20px;
    }
    .hero-text h1 {
        font-size: 2rem;
    }
}
