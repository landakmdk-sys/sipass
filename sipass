<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SIPAS – Sistem Informasi Persampahan</title>
<link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&family=DM+Serif+Display:ital@0;1&display=swap" rel="stylesheet">
<style>
  :root {
    --green-deep: #1a4a2e;
    --green-mid: #2d7a4f;
    --green-bright: #4caf50;
    --green-light: #a8e6b8;
    --green-pale: #e8f5ec;
    --amber: #f59e0b;
    --amber-light: #fef3c7;
    --red-soft: #ef4444;
    --blue-soft: #3b82f6;
    --cream: #fafaf7;
    --text-dark: #1a2e1f;
    --text-mid: #3d5c47;
    --text-soft: #6b8a74;
    --white: #ffffff;
    --shadow-sm: 0 2px 8px rgba(26,74,46,0.08);
    --shadow-md: 0 8px 32px rgba(26,74,46,0.12);
    --shadow-lg: 0 20px 60px rgba(26,74,46,0.18);
    --radius: 16px;
    --radius-sm: 10px;
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }

  body {
    font-family: 'Plus Jakarta Sans', sans-serif;
    background: var(--cream);
    color: var(--text-dark);
    line-height: 1.6;
    overflow-x: hidden;
  }

  /* ─── NAV ─── */
  nav {
    position: sticky;
    top: 0;
    z-index: 100;
    background: rgba(250,250,247,0.92);
    backdrop-filter: blur(12px);
    border-bottom: 1px solid rgba(26,74,46,0.08);
    padding: 0 40px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 64px;
  }

  .nav-logo {
    display: flex;
    align-items: center;
    gap: 10px;
    font-weight: 800;
    font-size: 1.1rem;
    color: var(--green-deep);
    text-decoration: none;
  }

  .nav-logo .icon {
    width: 36px; height: 36px;
    background: var(--green-mid);
    border-radius: 10px;
    display: flex; align-items: center; justify-content: center;
    font-size: 18px;
  }

  .nav-links {
    display: flex;
    gap: 4px;
    list-style: none;
  }

  .nav-links a {
    text-decoration: none;
    color: var(--text-mid);
    font-size: 0.88rem;
    font-weight: 500;
    padding: 7px 14px;
    border-radius: 8px;
    transition: all 0.2s;
  }

  .nav-links a:hover { background: var(--green-pale); color: var(--green-deep); }

  .nav-cta {
    background: var(--green-mid);
    color: white !important;
    padding: 8px 18px !important;
    border-radius: 20px !important;
  }

  .nav-cta:hover { background: var(--green-deep) !important; color: white !important; }

  /* ─── HERO ─── */
  .hero {
    position: relative;
    min-height: 88vh;
    display: flex;
    align-items: center;
    overflow: hidden;
    padding: 80px 40px;
  }

  .hero-bg {
    position: absolute; inset: 0;
    background: linear-gradient(135deg, var(--green-deep) 0%, #1e5c38 60%, #2d7a4f 100%);
  }

  .hero-pattern {
    position: absolute; inset: 0;
    background-image:
      radial-gradient(circle at 20% 50%, rgba(76,175,80,0.15) 0%, transparent 50%),
      radial-gradient(circle at 80% 20%, rgba(168,230,184,0.1) 0%, transparent 40%),
      radial-gradient(circle at 60% 80%, rgba(45,122,79,0.2) 0%, transparent 50%);
  }

  .hero-grid {
    position: absolute; inset: 0;
    background-image: linear-gradient(rgba(255,255,255,0.03) 1px, transparent 1px),
                      linear-gradient(90deg, rgba(255,255,255,0.03) 1px, transparent 1px);
    background-size: 40px 40px;
  }

  .hero-content {
    position: relative;
    max-width: 1200px;
    margin: 0 auto;
    width: 100%;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 80px;
    align-items: center;
  }

  .hero-left { }

  .hero-badge {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    background: rgba(255,255,255,0.12);
    border: 1px solid rgba(255,255,255,0.2);
    color: var(--green-light);
    font-size: 0.78rem;
    font-weight: 600;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    padding: 6px 14px;
    border-radius: 20px;
    margin-bottom: 24px;
  }

  .hero h1 {
    font-family: 'DM Serif Display', serif;
    font-size: clamp(2.4rem, 4vw, 3.6rem);
    color: white;
    line-height: 1.12;
    margin-bottom: 20px;
  }

  .hero h1 em {
    font-style: italic;
    color: var(--green-light);
  }

  .hero p {
    color: rgba(255,255,255,0.72);
    font-size: 1rem;
    max-width: 440px;
    margin-bottom: 36px;
    line-height: 1.7;
  }

  .hero-actions {
    display: flex;
    gap: 12px;
    flex-wrap: wrap;
  }

  .btn-primary {
    background: white;
    color: var(--green-deep);
    padding: 13px 26px;
    border-radius: 30px;
    font-weight: 700;
    font-size: 0.9rem;
    text-decoration: none;
    border: none;
    cursor: pointer;
    transition: all 0.25s;
    display: inline-flex;
    align-items: center;
    gap: 8px;
    box-shadow: 0 4px 20px rgba(0,0,0,0.2);
  }

  .btn-primary:hover { transform: translateY(-2px); box-shadow: 0 8px 30px rgba(0,0,0,0.25); }

  .btn-outline {
    background: transparent;
    color: white;
    padding: 13px 26px;
    border-radius: 30px;
    font-weight: 600;
    font-size: 0.9rem;
    text-decoration: none;
    border: 1.5px solid rgba(255,255,255,0.4);
    cursor: pointer;
    transition: all 0.25s;
    display: inline-flex;
    align-items: center;
    gap: 8px;
  }

  .btn-outline:hover { border-color: white; background: rgba(255,255,255,0.1); }

  .hero-right {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 16px;
  }

  .hero-stat-card {
    background: rgba(255,255,255,0.1);
    border: 1px solid rgba(255,255,255,0.15);
    border-radius: var(--radius);
    padding: 24px 20px;
    backdrop-filter: blur(8px);
    animation: floatCard 4s ease-in-out infinite;
  }

  .hero-stat-card:nth-child(2) { animation-delay: 0.5s; margin-top: 20px; }
  .hero-stat-card:nth-child(3) { animation-delay: 1s; }
  .hero-stat-card:nth-child(4) { animation-delay: 1.5s; margin-top: 20px; }

  @keyframes floatCard {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-6px); }
  }

  .hero-stat-card .emoji { font-size: 2rem; margin-bottom: 10px; display: block; }
  .hero-stat-card .num {
    font-family: 'DM Serif Display', serif;
    font-size: 2rem;
    color: white;
    display: block;
  }
  .hero-stat-card .label { color: rgba(255,255,255,0.65); font-size: 0.78rem; font-weight: 500; }

  /* ─── SECTION COMMON ─── */
  section { padding: 80px 40px; }
  .container { max-width: 1200px; margin: 0 auto; }

  .section-header { text-align: center; margin-bottom: 56px; }
  .section-tag {
    display: inline-block;
    background: var(--green-pale);
    color: var(--green-mid);
    font-size: 0.75rem;
    font-weight: 700;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    padding: 5px 14px;
    border-radius: 20px;
    margin-bottom: 14px;
  }
  .section-header h2 {
    font-family: 'DM Serif Display', serif;
    font-size: clamp(1.8rem, 3vw, 2.6rem);
    color: var(--green-deep);
    margin-bottom: 14px;
  }
  .section-header p { color: var(--text-soft); font-size: 0.97rem; max-width: 520px; margin: 0 auto; }

  /* ─── STATS STRIP ─── */
  .stats-strip {
    background: white;
    padding: 0 40px;
    border-top: 1px solid rgba(26,74,46,0.06);
    border-bottom: 1px solid rgba(26,74,46,0.06);
  }

  .stats-strip .container {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    divide-x: 1px solid var(--green-pale);
  }

  .stat-item {
    padding: 32px 24px;
    text-align: center;
    border-right: 1px solid var(--green-pale);
  }
  .stat-item:last-child { border-right: none; }

  .stat-item .num {
    font-family: 'DM Serif Display', serif;
    font-size: 2.6rem;
    color: var(--green-mid);
    display: block;
    line-height: 1;
    margin-bottom: 6px;
  }
  .stat-item .label { color: var(--text-soft); font-size: 0.82rem; font-weight: 500; }

  /* ─── JENIS SAMPAH ─── */
  .jenis-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 24px;
  }

  .jenis-card {
    background: white;
    border-radius: var(--radius);
    padding: 32px 28px;
    box-shadow: var(--shadow-sm);
    border: 1px solid transparent;
    transition: all 0.3s;
    position: relative;
    overflow: hidden;
  }

  .jenis-card::before {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 4px;
  }

  .jenis-card.organik::before { background: var(--green-bright); }
  .jenis-card.anorganik::before { background: var(--blue-soft); }
  .jenis-card.b3::before { background: var(--red-soft); }
  .jenis-card.daur-ulang::before { background: var(--amber); }
  .jenis-card.residu::before { background: #8b5cf6; }
  .jenis-card.elektronik::before { background: #06b6d4; }

  .jenis-card:hover {
    transform: translateY(-4px);
    box-shadow: var(--shadow-md);
    border-color: var(--green-pale);
  }

  .jenis-icon {
    width: 56px; height: 56px;
    border-radius: 14px;
    display: flex; align-items: center; justify-content: center;
    font-size: 28px;
    margin-bottom: 18px;
  }

  .jenis-card.organik .jenis-icon { background: #dcfce7; }
  .jenis-card.anorganik .jenis-icon { background: #dbeafe; }
  .jenis-card.b3 .jenis-icon { background: #fee2e2; }
  .jenis-card.daur-ulang .jenis-icon { background: #fef3c7; }
  .jenis-card.residu .jenis-icon { background: #ede9fe; }
  .jenis-card.elektronik .jenis-icon { background: #cffafe; }

  .jenis-card h3 {
    font-size: 1.05rem;
    font-weight: 700;
    color: var(--text-dark);
    margin-bottom: 8px;
  }

  .jenis-card p { color: var(--text-soft); font-size: 0.85rem; line-height: 1.6; margin-bottom: 14px; }

  .jenis-examples {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
  }

  .tag {
    background: var(--green-pale);
    color: var(--green-mid);
    font-size: 0.72rem;
    font-weight: 600;
    padding: 3px 10px;
    border-radius: 20px;
  }

  /* ─── JADWAL ─── */
  .jadwal-section { background: var(--green-pale); }

  .jadwal-grid {
    display: grid;
    grid-template-columns: repeat(7, 1fr);
    gap: 12px;
  }

  .jadwal-day {
    background: white;
    border-radius: var(--radius-sm);
    padding: 16px 12px;
    text-align: center;
    box-shadow: var(--shadow-sm);
    transition: all 0.25s;
    cursor: default;
  }

  .jadwal-day.active {
    background: var(--green-mid);
    color: white;
    transform: translateY(-4px);
    box-shadow: var(--shadow-md);
  }

  .jadwal-day .day-name {
    font-size: 0.72rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.08em;
    margin-bottom: 8px;
    opacity: 0.6;
  }

  .jadwal-day.active .day-name { opacity: 0.85; }

  .jadwal-day .day-icon { font-size: 1.8rem; display: block; margin-bottom: 8px; }

  .jadwal-day .day-type {
    font-size: 0.72rem;
    font-weight: 600;
    color: var(--text-soft);
  }

  .jadwal-day.active .day-type { color: rgba(255,255,255,0.85); }

  .jadwal-info {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
    margin-top: 32px;
  }

  .info-card {
    background: white;
    border-radius: var(--radius);
    padding: 24px;
    box-shadow: var(--shadow-sm);
    display: flex;
    gap: 16px;
    align-items: flex-start;
  }

  .info-icon {
    width: 44px; height: 44px;
    background: var(--green-pale);
    border-radius: 12px;
    display: flex; align-items: center; justify-content: center;
    font-size: 20px;
    flex-shrink: 0;
  }

  .info-card h4 { font-weight: 700; font-size: 0.92rem; color: var(--text-dark); margin-bottom: 4px; }
  .info-card p { color: var(--text-soft); font-size: 0.82rem; line-height: 1.5; }

  /* ─── CARA PILAH ─── */
  .steps {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 0;
    position: relative;
  }

  .steps::before {
    content: '';
    position: absolute;
    top: 44px;
    left: 12%;
    right: 12%;
    height: 2px;
    background: linear-gradient(90deg, var(--green-light), var(--green-mid));
    z-index: 0;
  }

  .step {
    text-align: center;
    padding: 0 16px;
    position: relative;
    z-index: 1;
  }

  .step-num {
    width: 56px; height: 56px;
    background: var(--green-mid);
    color: white;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: 'DM Serif Display', serif;
    font-size: 1.4rem;
    margin: 0 auto 20px;
    box-shadow: 0 0 0 6px var(--cream), 0 0 0 8px var(--green-light);
    transition: all 0.3s;
  }

  .step:hover .step-num {
    background: var(--green-deep);
    transform: scale(1.1);
  }

  .step h4 { font-weight: 700; color: var(--green-deep); margin-bottom: 8px; font-size: 0.95rem; }
  .step p { color: var(--text-soft); font-size: 0.83rem; line-height: 1.6; }

  /* ─── KONTAK ─── */
  .kontak-section { background: var(--green-deep); }

  .kontak-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 60px;
    align-items: start;
  }

  .kontak-left h2 {
    font-family: 'DM Serif Display', serif;
    font-size: 2.2rem;
    color: white;
    margin-bottom: 16px;
  }

  .kontak-left p { color: rgba(255,255,255,0.65); font-size: 0.93rem; margin-bottom: 32px; }

  .kontak-items { display: flex; flex-direction: column; gap: 16px; }

  .kontak-item {
    display: flex;
    gap: 14px;
    align-items: center;
  }

  .kontak-item-icon {
    width: 44px; height: 44px;
    background: rgba(255,255,255,0.1);
    border-radius: 12px;
    display: flex; align-items: center; justify-content: center;
    font-size: 20px;
    flex-shrink: 0;
  }

  .kontak-item span { color: rgba(255,255,255,0.85); font-size: 0.9rem; }
  .kontak-item strong { color: white; display: block; font-size: 0.85rem; margin-bottom: 2px; }

  .kontak-form {
    background: white;
    border-radius: var(--radius);
    padding: 36px;
  }

  .kontak-form h3 {
    font-weight: 700;
    color: var(--green-deep);
    margin-bottom: 24px;
    font-size: 1.1rem;
  }

  .form-group { margin-bottom: 18px; }

  .form-group label {
    display: block;
    font-size: 0.8rem;
    font-weight: 600;
    color: var(--text-mid);
    margin-bottom: 6px;
    text-transform: uppercase;
    letter-spacing: 0.05em;
  }

  .form-group input,
  .form-group select,
  .form-group textarea {
    width: 100%;
    padding: 11px 14px;
    border: 1.5px solid rgba(26,74,46,0.15);
    border-radius: var(--radius-sm);
    font-family: inherit;
    font-size: 0.9rem;
    color: var(--text-dark);
    background: var(--cream);
    transition: all 0.2s;
    outline: none;
  }

  .form-group input:focus,
  .form-group select:focus,
  .form-group textarea:focus {
    border-color: var(--green-mid);
    background: white;
    box-shadow: 0 0 0 3px rgba(45,122,79,0.1);
  }

  .form-group textarea { resize: vertical; min-height: 90px; }

  .btn-submit {
    width: 100%;
    background: var(--green-mid);
    color: white;
    border: none;
    padding: 13px;
    border-radius: 10px;
    font-family: inherit;
    font-size: 0.92rem;
    font-weight: 700;
    cursor: pointer;
    transition: all 0.25s;
    margin-top: 8px;
  }

  .btn-submit:hover { background: var(--green-deep); transform: translateY(-1px); }

  /* ─── PENGUMUMAN ─── */
  .pengumuman-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 24px;
  }

  .news-card {
    background: white;
    border-radius: var(--radius);
    overflow: hidden;
    box-shadow: var(--shadow-sm);
    transition: all 0.3s;
  }

  .news-card:hover { transform: translateY(-4px); box-shadow: var(--shadow-md); }

  .news-img {
    height: 160px;
    background: linear-gradient(135deg, var(--green-mid), var(--green-deep));
    display: flex; align-items: center; justify-content: center;
    font-size: 4rem;
  }

  .news-body { padding: 20px; }

  .news-meta {
    display: flex;
    gap: 10px;
    align-items: center;
    margin-bottom: 10px;
  }

  .news-cat {
    background: var(--green-pale);
    color: var(--green-mid);
    font-size: 0.7rem;
    font-weight: 700;
    padding: 3px 10px;
    border-radius: 20px;
  }

  .news-date { color: var(--text-soft); font-size: 0.75rem; }

  .news-card h4 {
    font-weight: 700;
    color: var(--text-dark);
    font-size: 0.95rem;
    margin-bottom: 8px;
    line-height: 1.4;
  }

  .news-card p { color: var(--text-soft); font-size: 0.82rem; line-height: 1.6; }

  /* ─── FOOTER ─── */
  footer {
    background: #0f2e1c;
    color: rgba(255,255,255,0.5);
    text-align: center;
    padding: 28px 40px;
    font-size: 0.82rem;
  }

  footer strong { color: rgba(255,255,255,0.85); }

  /* ─── RESPONSIVE ─── */
  @media (max-width: 900px) {
    .hero-content { grid-template-columns: 1fr; gap: 40px; }
    .hero-right { grid-template-columns: repeat(2, 1fr); }
    .hero-stat-card:nth-child(2), .hero-stat-card:nth-child(4) { margin-top: 0; }
    .stats-strip .container { grid-template-columns: repeat(2, 1fr); }
    .jenis-grid { grid-template-columns: 1fr 1fr; }
    .jadwal-grid { grid-template-columns: repeat(4, 1fr); }
    .steps { grid-template-columns: 1fr 1fr; }
    .steps::before { display: none; }
    .kontak-grid { grid-template-columns: 1fr; }
    .pengumuman-grid { grid-template-columns: 1fr; }
    nav { padding: 0 20px; }
    .nav-links { display: none; }
  }

  /* ─── ANIMATIONS ─── */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(24px); }
    to { opacity: 1; transform: translateY(0); }
  }

  .hero-badge { animation: fadeUp 0.6s ease both; }
  .hero h1 { animation: fadeUp 0.6s 0.1s ease both; }
  .hero p { animation: fadeUp 0.6s 0.2s ease both; }
  .hero-actions { animation: fadeUp 0.6s 0.3s ease both; }
</style>
</head>
<body>

<!-- ─── NAV ─── -->
<nav>
  <a class="nav-logo" href="#">
    <div class="icon">♻️</div>
    SIPAS
  </a>
  <ul class="nav-links">
    <li><a href="#jenis">Jenis Sampah</a></li>
    <li><a href="#jadwal">Jadwal</a></li>
    <li><a href="#cara-pilah">Cara Pilah</a></li>
    <li><a href="#pengumuman">Pengumuman</a></li>
    <li><a href="#kontak" class="nav-cta">Lapor</a></li>
  </ul>
</nav>

<!-- ─── HERO ─── -->
<section class="hero">
  <div class="hero-bg"></div>
  <div class="hero-pattern"></div>
  <div class="hero-grid"></div>

  <div class="hero-content">
    <div class="hero-left">
      <div class="hero-badge">🌿 Dinas Lingkungan Hidup</div>
      <h1>Bersama Jaga <em>Kebersihan</em> Kota Kita</h1>
      <p>Sistem Informasi Persampahan terpadu untuk memudahkan masyarakat dalam pengelolaan sampah, jadwal pengangkutan, dan pelaporan masalah lingkungan.</p>
      <div class="hero-actions">
        <a href="#jadwal" class="btn-primary">📅 Lihat Jadwal</a>
        <a href="#kontak" class="btn-outline">📋 Buat Laporan</a>
      </div>
    </div>

    <div class="hero-right">
      <div class="hero-stat-card">
        <span class="emoji">🏠</span>
        <span class="num">48.2K</span>
        <span class="label">KK Terlayani</span>
      </div>
      <div class="hero-stat-card">
        <span class="emoji">🚛</span>
        <span class="num">24</span>
        <span class="label">Armada Aktif</span>
      </div>
      <div class="hero-stat-card">
        <span class="emoji">♻️</span>
        <span class="num">68%</span>
        <span class="label">Daur Ulang</span>
      </div>
      <div class="hero-stat-card">
        <span class="emoji">📍</span>
        <span class="num">12</span>
        <span class="label">Titik TPS</span>
      </div>
    </div>
  </div>
</section>

<!-- ─── STATS STRIP ─── -->
<div class="stats-strip">
  <div class="container">
    <div class="stat-item">
      <span class="num">142t</span>
      <span class="label">Sampah Terangkut / Hari</span>
    </div>
    <div class="stat-item">
      <span class="num">96%</span>
      <span class="label">Cakupan Layanan</span>
    </div>
    <div class="stat-item">
      <span class="num">3.200</span>
      <span class="label">Laporan Ditangani</span>
    </div>
    <div class="stat-item">
      <span class="num">8 Kel</span>
      <span class="label">Wilayah Terlayani</span>
    </div>
  </div>
</div>

<!-- ─── JENIS SAMPAH ─── -->
<section id="jenis">
  <div class="container">
    <div class="section-header">
      <span class="section-tag">Edukasi</span>
      <h2>Jenis Sampah & Penanganannya</h2>
      <p>Kenali jenis sampah agar dapat dibuang dan dikelola dengan tepat untuk lingkungan yang lebih baik.</p>
    </div>

    <div class="jenis-grid">
      <div class="jenis-card organik">
        <div class="jenis-icon">🥦</div>
        <h3>Sampah Organik</h3>
        <p>Sampah yang mudah terurai secara alami dari bahan-bahan makhluk hidup.</p>
        <div class="jenis-examples">
          <span class="tag">Sisa makanan</span>
          <span class="tag">Daun kering</span>
          <span class="tag">Kulit buah</span>
          <span class="tag">Kotoran hewan</span>
        </div>
      </div>

      <div class="jenis-card anorganik">
        <div class="jenis-icon">🧴</div>
        <h3>Sampah Anorganik</h3>
        <p>Sampah yang sulit atau tidak dapat terurai secara alami, perlu penanganan khusus.</p>
        <div class="jenis-examples">
          <span class="tag">Plastik</span>
          <span class="tag">Kaca</span>
          <span class="tag">Logam</span>
          <span class="tag">Styrofoam</span>
        </div>
      </div>

      <div class="jenis-card daur-ulang">
        <div class="jenis-icon">📦</div>
        <h3>Sampah Daur Ulang</h3>
        <p>Sampah yang dapat diolah kembali menjadi bahan baku atau produk baru.</p>
        <div class="jenis-examples">
          <span class="tag">Kertas</span>
          <span class="tag">Kardus</span>
          <span class="tag">Botol PET</span>
          <span class="tag">Kaleng</span>
        </div>
      </div>

      <div class="jenis-card b3">
        <div class="jenis-icon">⚠️</div>
        <h3>Sampah B3</h3>
        <p>Sampah Bahan Berbahaya dan Beracun yang memerlukan penanganan khusus dan aman.</p>
        <div class="jenis-examples">
          <span class="tag">Baterai</span>
          <span class="tag">Obat kadaluarsa</span>
          <span class="tag">Cat</span>
          <span class="tag">Pestisida</span>
        </div>
      </div>

      <div class="jenis-card residu">
        <div class="jenis-icon">🗑️</div>
        <h3>Sampah Residu</h3>
        <p>Sampah yang tidak dapat didaur ulang dan harus dibuang ke TPA setelah dipilah.</p>
        <div class="jenis-examples">
          <span class="tag">Pampers</span>
          <span class="tag">Popok</span>
          <span class="tag">Tisu kotor</span>
          <span class="tag">Pembalut</span>
        </div>
      </div>

      <div class="jenis-card elektronik">
        <div class="jenis-icon">📱</div>
        <h3>Sampah Elektronik</h3>
        <p>Perangkat elektronik bekas yang mengandung komponen berbahaya jika dibuang sembarangan.</p>
        <div class="jenis-examples">
          <span class="tag">Handphone</span>
          <span class="tag">Laptop</span>
          <span class="tag">Kabel</span>
          <span class="tag">Charger</span>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ─── JADWAL ─── -->
<section id="jadwal" class="jadwal-section">
  <div class="container">
    <div class="section-header">
      <span class="section-tag">Jadwal</span>
      <h2>Jadwal Pengangkutan Sampah</h2>
      <p>Pastikan sampah sudah diletakkan di depan rumah sebelum pukul 06.00 WIB pada hari yang dijadwalkan.</p>
    </div>

    <div class="jadwal-grid">
      <div class="jadwal-day">
        <div class="day-name">Sen</div>
        <span class="day-icon">🥦</span>
        <div class="day-type">Organik</div>
      </div>
      <div class="jadwal-day">
        <div class="day-name">Sel</div>
        <span class="day-icon">♻️</span>
        <div class="day-type">Daur Ulang</div>
      </div>
      <div class="jadwal-day">
        <div class="day-name">Rab</div>
        <span class="day-icon">🥦</span>
        <div class="day-type">Organik</div>
      </div>
      <div class="jadwal-day active">
        <div class="day-name">Kam</div>
        <span class="day-icon">🗑️</span>
        <div class="day-type">Residu</div>
      </div>
      <div class="jadwal-day">
        <div class="day-name">Jum</div>
        <span class="day-icon">🥦</span>
        <div class="day-type">Organik</div>
      </div>
      <div class="jadwal-day">
        <div class="day-name">Sab</div>
        <span class="day-icon">📦</span>
        <div class="day-type">Anorganik</div>
      </div>
      <div class="jadwal-day">
        <div class="day-name">Min</div>
        <span class="day-icon">🚫</span>
        <div class="day-type">Libur</div>
      </div>
    </div>

    <div class="jadwal-info">
      <div class="info-card">
        <div class="info-icon">⏰</div>
        <div>
          <h4>Waktu Pengangkutan</h4>
          <p>Armada beroperasi mulai pukul 06.00 – 12.00 WIB. Sampah harus sudah di depan rumah sebelum jam 06.00 WIB.</p>
        </div>
      </div>
      <div class="info-card">
        <div class="info-icon">📍</div>
        <div>
          <h4>Lokasi TPS Terdekat</h4>
          <p>Temukan TPS (Tempat Pembuangan Sementara) dan bank sampah terdekat di wilayah Anda melalui fitur peta.</p>
        </div>
      </div>
      <div class="info-card">
        <div class="info-icon">🚛</div>
        <div>
          <h4>Lacak Armada</h4>
          <p>Pantau posisi truk sampah secara real-time agar Anda tahu kapan armada tiba di lingkungan Anda.</p>
        </div>
      </div>
      <div class="info-card">
        <div class="info-icon">📅</div>
        <div>
          <h4>Jadwal Khusus Hari Raya</h4>
          <p>Pada hari libur nasional, jadwal pengangkutan mungkin berubah. Pantau pengumuman terkini di situs ini.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ─── CARA PILAH ─── -->
<section id="cara-pilah">
  <div class="container">
    <div class="section-header">
      <span class="section-tag">Panduan</span>
      <h2>Cara Memilah Sampah yang Benar</h2>
      <p>Empat langkah mudah untuk memilah sampah di rumah tangga dan berkontribusi nyata pada lingkungan.</p>
    </div>

    <div class="steps">
      <div class="step">
        <div class="step-num">1</div>
        <h4>Siapkan Wadah Terpisah</h4>
        <p>Sediakan minimal 3 tempat sampah berbeda untuk organik, anorganik, dan residu di rumah Anda.</p>
      </div>
      <div class="step">
        <div class="step-num">2</div>
        <h4>Pilah Saat Membuang</h4>
        <p>Biasakan langsung pilah sampah sesuai jenisnya saat hendak dibuang, bukan dikumpulkan dulu.</p>
      </div>
      <div class="step">
        <div class="step-num">3</div>
        <h4>Bersihkan Sebelum Buang</h4>
        <p>Bilas wadah plastik atau kaca sebelum dibuang ke tempat daur ulang agar tidak mencemari sampah lain.</p>
      </div>
      <div class="step">
        <div class="step-num">4</div>
        <h4>Buang Sesuai Jadwal</h4>
        <p>Keluarkan sampah pada hari yang telah dijadwalkan sesuai jenis sampah yang akan diangkut.</p>
      </div>
    </div>
  </div>
</section>

<!-- ─── PENGUMUMAN ─── -->
<section id="pengumuman" style="background: white;">
  <div class="container">
    <div class="section-header">
      <span class="section-tag">Berita</span>
      <h2>Pengumuman & Kegiatan</h2>
      <p>Informasi terkini seputar kegiatan kebersihan dan program lingkungan di wilayah kita.</p>
    </div>

    <div class="pengumuman-grid">
      <div class="news-card">
        <div class="news-img">🌿</div>
        <div class="news-body">
          <div class="news-meta">
            <span class="news-cat">Program</span>
            <span class="news-date">15 Maret 2025</span>
          </div>
          <h4>Peluncuran Bank Sampah Digital Kecamatan</h4>
          <p>Program bank sampah digital kini hadir di 5 kelurahan untuk memudahkan warga menukar sampah daur ulang menjadi poin reward.</p>
        </div>
      </div>

      <div class="news-card">
        <div class="news-img">🚛</div>
        <div class="news-body">
          <div class="news-meta">
            <span class="news-cat">Pengumuman</span>
            <span class="news-date">10 Maret 2025</span>
          </div>
          <h4>Perubahan Jadwal Pengangkutan Selama Ramadan</h4>
          <p>Selama bulan Ramadan, jadwal pengangkutan sampah disesuaikan menjadi pukul 04.30 WIB untuk wilayah pasar dan pusat kota.</p>
        </div>
      </div>

      <div class="news-card">
        <div class="news-img">♻️</div>
        <div class="news-body">
          <div class="news-meta">
            <span class="news-cat">Kegiatan</span>
            <span class="news-date">5 Maret 2025</span>
          </div>
          <h4>Kerja Bakti Massal 5.000 Warga Bersihkan Sungai</h4>
          <p>Kegiatan bersih sungai melibatkan ribuan warga berhasil mengangkat lebih dari 8 ton sampah dari aliran sungai kota.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ─── KONTAK ─── -->
<section id="kontak" class="kontak-section">
  <div class="container">
    <div class="kontak-grid">
      <div class="kontak-left">
        <h2>Hubungi & Laporkan Masalah</h2>
        <p>Temukan tumpukan sampah liar? Ada armada yang tidak beroperasi? Laporkan kepada kami dan tim akan segera menindaklanjuti.</p>
        <div class="kontak-items">
          <div class="kontak-item">
            <div class="kontak-item-icon">📞</div>
            <div>
              <strong>Hotline 24 Jam</strong>
              <span>(0451) 123-4567 / 082-xxxx-xxxx</span>
            </div>
          </div>
          <div class="kontak-item">
            <div class="kontak-item-icon">📧</div>
            <div>
              <strong>Email</strong>
              <span>persampahan@dinlh.go.id</span>
            </div>
          </div>
          <div class="kontak-item">
            <div class="kontak-item-icon">📍</div>
            <div>
              <strong>Kantor DLH</strong>
              <span>Jl. Lingkungan Hidup No. 1, Kota</span>
            </div>
          </div>
          <div class="kontak-item">
            <div class="kontak-item-icon">🕐</div>
            <div>
              <strong>Jam Pelayanan</strong>
              <span>Senin – Jumat: 08.00 – 16.00 WIB</span>
            </div>
          </div>
        </div>
      </div>

      <div class="kontak-form">
        <h3>📋 Form Pelaporan</h3>
        <div class="form-group">
          <label>Nama Lengkap</label>
          <input type="text" placeholder="Masukkan nama Anda">
        </div>
        <div class="form-group">
          <label>Nomor HP</label>
          <input type="tel" placeholder="08xx-xxxx-xxxx">
        </div>
        <div class="form-group">
          <label>Jenis Laporan</label>
          <select>
            <option value="">– Pilih Jenis Laporan –</option>
            <option>Tumpukan sampah liar</option>
            <option>Armada tidak datang</option>
            <option>TPS penuh / meluap</option>
            <option>Pembuangan sampah B3</option>
            <option>Saran & masukan</option>
            <option>Lainnya</option>
          </select>
        </div>
        <div class="form-group">
          <label>Lokasi Kejadian</label>
          <input type="text" placeholder="Alamat / nama tempat kejadian">
        </div>
        <div class="form-group">
          <label>Keterangan</label>
          <textarea placeholder="Deskripsikan masalah yang ingin dilaporkan..."></textarea>
        </div>
        <button class="btn-submit" onclick="alert('Laporan berhasil dikirim! Tim kami akan menindaklanjuti dalam 1×24 jam. Terima kasih!')">
          Kirim Laporan →
        </button>
      </div>
    </div>
  </div>
</section>

<!-- ─── FOOTER ─── -->
<footer>
  <p>© 2025 <strong>SIPAS – Sistem Informasi Persampahan</strong> · Dinas Lingkungan Hidup · Dibuat untuk lingkungan yang lebih bersih 🌿</p>
</footer>

</body>
</html>
