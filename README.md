<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lintas Sulawesi | Premium Travel & VIP Service</title>
    
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;600;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css">
    
    <style>
        :root {
            --primary: #3b82f6; 
            --accent: #facc15; 
            --text-main: #f8fafc;
            --card-bg: rgba(30, 41, 59, 0.6); 
        }

        html { scroll-behavior: smooth; }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Plus Jakarta Sans', sans-serif; }
        
        body { 
            margin: 0;
            padding-bottom: 150px; /* Ruang ekstra untuk nav besar */
            color: var(--text-main);
            background: linear-gradient(-45deg, #0f172a, #1e1b4b, #2e1065, #020617);
            background-size: 400% 400%;
            animation: darkGradient 12s ease infinite;
            min-height: 100vh;
        }

        @keyframes darkGradient {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .container { max-width: 800px; margin: 0 auto; padding: 20px; }

        .hero { padding: 60px 20px 40px; text-align: center; }
        .hero h1 { font-size: 2.2rem; font-weight: 800; letter-spacing: -1px; }

        .card {
            background: var(--card-bg);
            backdrop-filter: blur(20px);
            border-radius: 30px;
            padding: 25px;
            margin-bottom: 25px;
            border: 1px solid rgba(255, 255, 255, 0.08);
        }

        h2 { font-size: 1.2rem; margin-bottom: 20px; display: flex; align-items: center; gap: 10px; color: var(--primary); }

        /* TESTIMONI */
        .testi-grid { display: flex; overflow-x: auto; gap: 15px; padding-bottom: 10px; scrollbar-width: none; }
        .testi-item { min-width: 250px; background: rgba(255,255,255,0.05); padding: 15px; border-radius: 20px; border: 1px solid rgba(255,255,255,0.05); }
        .testi-item p { font-size: 0.8rem; font-style: italic; margin-bottom: 10px; color: #cbd5e1; }
        .testi-user { font-size: 0.75rem; font-weight: 800; color: var(--accent); }

        /* FAQ */
        .faq-item { margin-bottom: 15px; background: rgba(0,0,0,0.2); padding: 15px; border-radius: 15px; }
        .faq-item b { font-size: 0.85rem; color: var(--primary); display: block; margin-bottom: 5px; }
        .faq-item p { font-size: 0.8rem; color: #94a3b8; }

        /* HARGA TABLE */
        .price-table { width: 100%; border-collapse: collapse; }
        .price-table td { padding: 12px; border-bottom: 1px solid rgba(255,255,255,0.05); font-size: 0.85rem; }
        .val-vip { color: var(--accent); font-weight: 800; text-align: right; }

        /* FORM */
        .field { margin-bottom: 15px; }
        label { font-size: 0.75rem; color: #94a3b8; font-weight: 700; display: block; margin-bottom: 5px; }
        input, select, textarea { 
            width: 100%; padding: 15px; border-radius: 15px; border: 1px solid rgba(255,255,255,0.1); 
            background: rgba(15, 23, 42, 0.8); color: white; outline: none;
        }
        .btn-kirim {
            background: var(--primary); color: white; padding: 18px; border: none; 
            border-radius: 15px; font-weight: 800; cursor: pointer; width: 100%;
        }

        /* FLOATING NAV (MODERN & BESAR) */
        .bottom-nav {
            position: fixed; bottom: 30px; left: 50%; transform: translateX(-50%);
            width: 90%; max-width: 450px; background: rgba(15, 23, 42, 0.9);
            backdrop-filter: blur(20px); display: flex; justify-content: space-between; align-items: center;
            padding: 10px 25px; border-radius: 40px; border: 1px solid rgba(255,255,255,0.1); z-index: 9999;
            box-shadow: 0 20px 40px rgba(0,0,0,0.6);
        }
        .nav-item { color: #64748b; text-decoration: none; text-align: center; font-size: 0.7rem; transition: 0.3s; }
        .nav-item i { display: block; font-size: 1.4rem; margin-bottom: 3px; }

        /* TOMBOL TENGAH BESAR */
        .nav-main {
            background: var(--primary); color: white !important;
            width: 70px; height: 70px; border-radius: 50%;
            display: flex; flex-direction: column; align-items: center; justify-content: center;
            margin-top: -45px; border: 5px solid #0f172a;
            box-shadow: 0 10px 20px rgba(59, 130, 246, 0.4);
        }
        .nav-main i { font-size: 1.8rem !important; margin: 0 !important; }

        /* EFEK WARNA SAAT DIPENCET */
        .nav-item:active, .nav-item.active-link { color: var(--accent); transform: scale(0.9); }
        .nav-main:active { background: var(--accent); transform: scale(0.9) translateY(-40px); }

    </style>
</head>
<body>

<div class="hero" id="home">
    <h1>LINTAS SULAWESI</h1>
    <p style="color: var(--primary); font-weight: 700;">Premium Executive Travel</p>
</div>

<div class="container">
    
    <div class="card" id="tentang">
        <h2><i class="fas fa-gem"></i> Keunggulan</h2>
        <p style="font-size: 0.85rem; line-height: 1.6; color: #cbd5e1;">Layanan antar jemput rumah ke rumah dengan driver profesional yang ramah, sopan, dan unit kendaraan yang selalu prima (Full AC & Musik).</p>
    </div>

    <div class="card" id="harga">
        <h2><i class="fas fa-tags"></i> Tarif Per Kursi</h2>
        <table class="price-table">
            <tr><td>Wajo ↔ Makassar</td><td class="val-vip">Standar 200rb / VIP 220rb</td></tr>
            <tr><td>Wajo ↔ Sinjai</td><td class="val-vip">Standar 150rb / VIP 170rb</td></tr>
            <tr><td>Sinjai ↔ Makassar</td><td class="val-vip">Standar 180rb / VIP 200rb</td></tr>
        </table>
    </div>

    <div class="card">
        <h2><i class="fas fa-star"></i> Testimoni</h2>
        <div class="testi-grid">
            <div class="testi-item">
                <p>"Sangat nyaman, jemputnya tepat waktu dan sopirnya ramah sekali. Pajeronya mantap!"</p>
                <span class="testi-user">- Andi, Wajo</span>
            </div>
            <div class="testi-item">
                <p>"Travel langganan kalau ke Makassar. Mobil bersih dan tidak merokok di dalam."</p>
                <span class="testi-user">- Sari, Sinjai</span>
            </div>
            <div class="testi-item">
                <p>"Harga sesuai dengan kualitas. Driver sangat paham rute dan tidak ugal-ugalan."</p>
                <span class="testi-user">- Budi, Makassar</span>
            </div>
        </div>
    </div>

    <div class="card">
        <h2><i class="fas fa-question-circle"></i> FAQ</h2>
        <div class="faq-item">
            <b>Apakah bisa jemput di dalam lorong?</b>
            <p>Bisa, selama jalan bisa dilewati mobil kami antar jemput sampai depan rumah.</p>
        </div>
        <div class="faq-item">
            <b>Bagaimana jika ingin carter?</b>
            <p>Silakan hubungi admin via WhatsApp untuk mendapatkan harga spesial carter satu mobil.</p>
        </div>
    </div>

    <div class="card" id="pesan">
        <h2><i class="fas fa-clipboard-check"></i> Form Booking</h2>
        <div class="field"><label>Nama Lengkap</label><input type="text" id="nama" placeholder="Andi ..."></div>
        <div class="field">
            <label>Pilih Mobil</label>
            <select id="mobil">
                <option>Innova Reborn</option>
                <option>Pajero Sport (VIP)</option>
                <option>Toyota Veloz</option>
            </select>
        </div>
        <div class="field"><label>Alamat Penjemputan</label><textarea id="alamat" placeholder="Jl. ... Sengkang"></textarea></div>
        <button class="btn-kirim" onclick="kirimWA()">DAFTAR SEKARANG</button>
    </div>

</div>

<nav class="bottom-nav">
    <a href="#home" class="nav-item"><i class="fas fa-house"></i>Home</a>
    <a href="#harga" class="nav-item"><i class="fas fa-tags"></i>Tarif</a>
    <a href="#pesan" class="nav-item nav-main"><i class="fas fa-plus"></i>Pesan</a>
    <a href="#tentang" class="nav-item"><i class="fas fa-info-circle"></i>Info</a>
    <a href="https://wa.me/6281234567890" class="nav-item"><i class="fab fa-whatsapp"></i>Admin</a>
</nav>

<script>
    function kirimWA() {
        const n = document.getElementById('nama').value;
        const m = document.getElementById('mobil').value;
        const a = document.getElementById('alamat').value;

        if(!n || !a) { alert("Lengkapi Nama dan Alamat!"); return; }

        const nomor = "6281234567890"; // GANTI NOMOR ANDA
        const pesan = `*BOOKING LINTAS SULAWESI*%0A%0A👤 *Nama:* ${n}%0A🚗 *Mobil:* ${m}%0A🏠 *Alamat:* ${a}`;
        window.open(`https://wa.me/${nomor}?text=${pesan}`, '_blank');
    }

    // Menambah efek warna saat menu diklik
    const navItems = document.querySelectorAll('.nav-item');
    navItems.forEach(item => {
        item.addEventListener('click', function() {
            navItems.forEach(i => i.classList.remove('active-link'));
            this.classList.add('active-link');
        });
    });
</script>

</body>
</html>
