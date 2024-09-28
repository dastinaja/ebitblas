<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kenangan Kelas</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap');

        body {
            font-family: 'Times New Roman', Times, serif
            margin: 0;
            padding: 0;
            background-color: #F3F1F5;
            color: #2C2C2C;
            scroll-behavior: smooth; /* Menambahkan scroll yang halus */
        }

        header {
            background-image: url(dustin3.jpeg);
            color: white;
            padding: 2px 2px;
            text-align: center;
            font-size: 2.5rem;
            letter-spacing: 2px;
            font-weight: 600;
        }

        nav {
            display: flex;
            justify-content: center;
            background-color: #454444;
            padding: 30px;
        }

        nav a {
            color: #ffffff;
            padding: 10px 20px;
            text-decoration: none;
            text-transform: uppercase;
            margin: 0 15px;
            font-weight: 500;
            transition: color 0.10s ease;
            font-size: 1.1rem;
        }

        nav a:hover {
            color: #12e3fe;
        }

        .slideshow-container {
            position: relative;
            max-width: 100%;
            margin: auto;
            height: 450px;
            overflow: hidden;
        }

        .slideshow {
            display: none;
            height: 100%;
        }

        .slideshow img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .slideshow.active {
            display: block;
        }

        .prev, .next {
            cursor: pointer;
            position: absolute;
            top: 50%;
            width: auto;
            padding: 16px;
            color: white;
            font-weight: bold;
            font-size: 18px;
            transition: background-color 0.3s ease;
            user-select: none;
        }

        .next {
            right: 0;
        }

        .prev:hover, .next:hover {
            background-color: rgba(0,0,0,0.5);
        }

        /* Struktur Kelas */
        .structure {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin: 50px 0;
        }

        .structure-title {
            font-size: 2rem;
            color: #2C2C2C;
            margin-bottom: 20px;
        }

        .row {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
        }

        .card {
            background-color: white;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            padding: 20px;
            margin: 15px;
            border-radius: 10px;
            width: 300px;
            text-align: center;
            transition: transform 0.3s;
        }

        .card:hover {
            transform: scale(1.05);
        }

        .role {
            font-size: 1.3rem;
            font-weight: 600;
            color: #2C2C2C;
            margin-bottom: 10px;
        }

        .name {
            font-size: 1.1rem;
            font-weight: 400;
            color: #606060;
            margin-bottom: 15px;
        }

        .card img {
            border-radius: 50%;
            width: 100px;
            height: 100px;
            object-fit: cover;
            margin-bottom: 10px;
        }

        /* Contact and About Us */
        section {
            padding: 50px 20px;
        }

        #contact, #about-us {
            background-color: #A9D8B8;
            color: white;
            text-align: center;
            padding: 30px;
            margin-top: 30px;
        }

        #about-us h2, #contact h2 {
            margin-bottom: 20px;
        }

        #contact p {
            margin-bottom: 15px;
        }

        /* Jadwal Pelajaran */
        .schedule {
            width: 80%;
            margin: 0 auto;
            text-align: left;
        }

        .day-schedule {
            background-color: #A9D8B8;
            color: white;
            padding: 15px;
            margin-top: 30px;
            border-radius: 8px;
            font-size: 1.3rem;
            font-weight: 600;
            letter-spacing: 1px;
        }

        .subject-list {
            list-style-type: none;
            padding-left: 0;
            margin: 15px 0;
        }

        .subject-list li {
            background-color: #fff;
            padding: 15px;
            margin-bottom: 10px;
            border-radius: 8px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            color: #2C2C2C;
            font-size: 1.1rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        footer {
            color: white;
            text-align: center;
            padding: 30px 20px;
            background-color: #2C2C2C;
        }

        footer p {
            margin: 0;
            font-size: 1rem;
        }
    </style>
</head>
<body>

    <header>
        <h1>Ebitblas</h1>
    </header>

    
    <nav>
        <a href="#home">Home</a>
        <a href="#memories" id="memories-link">Memories</a>
        <a href="#struktur">Struktur</a>
        <a href="#jadwal">Jadwal</a>
        <a href="#about-us">About Us</a>
        <a href="#contact">Contact</a>
    </nav>
 
   

    <!-- Slideshow -->
    <div class="slideshow-container" id="home">
        <div class="slideshow active">
            <img src="dustin5.jpeg" alt="Kenangan 1">

        </div>
        <a class="prev" onclick="changeSlide(-1)">&#10094;</a>
        <a class="next" onclick="changeSlide(1)">&#10095;</a>
    </div>

    <!-- Memories Section -->
    <section id="memories">
        <div style="text-align: center; padding: 50px;">
            <h2>Memories</h2>
            <p>Berikut adalah kenangan-kenangan indah kita selama di kelas:</p>
            <img src="dustin1.jpeg" alt="Foto Kenangan 1" style="width: 30%; margin: 20px auto; border-radius: 50px;">
            <img src="dustin2.jpeg" alt="Foto Kenangan 2" style="width: 30%; margin: 20px auto; border-radius: 50px;">
            <img src="dustin3.jpeg" alt="Foto Kenangan 3" style="width: 30%; margin: 30px auto; border-radius: 50px;">
            <img src="dustin7.jpeg" alt="Foto Kenangan 3" style="width: 40%; margin: 40px auto; border-radius: 50px;">
            <img src="dustin4.jpeg" alt="Foto Kenangan 3" style="width: 40%; margin: 40px auto; border-radius:50px;">
            <img src="dustin6.jpeg" alt="Foto Kenangan 3" style="width: 40%; margin: 40px auto; border-radius: 50px;">
        </div>
    </section>

    <!-- Struktur Kelas -->
    <section id="struktur">
        <div class="structure">
            <h2 class="structure-title">STRUKTUR KELAS</h2>
    
            <!-- Wali Kelas di atas sendiri -->
            <div class="row">
                <div class="card">
                    <div class="role">WALI KELAS</div>
                    <div class="name">Handayani.S.Pd.i</div>
                </div>
            </div>
    
            <!-- Ketua Kelas dan Wakil Ketua Kelas disamping -->
            <div class="row">
                <div class="card">
                    <div class="role">KETUA KELAS</div>
                    <div class="name">Kamal Azamta</div>
                </div>
    
                <div class="card">
                    <div class="role">WAKIL KETUA</div>
                    <div class="name">Lahvia Anisah</div>
                </div>
            </div>
    
            <div class="row">
                <div class="card">
                    <div class="role">SEKRETARIS</div>
                    <div class="name">Ratu Raisya & Dinda Hanindiya</div>
                </div>
    
                <div class="card">
                    <div class="role">BENDAHARA</div>
                    <div class="name">Nilnamaya & Ihsani Aini</div>
                </div>
            </div>
    
            <div class="row">
                <div class="card">
                    <div class="role">KEAMANAN</div>
                    <div class="name">Dustin Alea & Sandy Tristiawan</div>
                </div>
    
                <div class="card">
                    <div class="role">KEAGAMAAN</div>
                    <div class="name">Muhammad Ribhan & Muhammad Alief</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Jadwal Pelajaran -->
    <div class="structure">
        <h2 class="structure-title">Jadwal Pelajaran</h2>
    <div class="schedule">
        <div class="day-schedule">Senin</div>
        <ul class="subject-list">
            <li><span>07:10 - 08:30</span> <span>Aqidah Akhlak</span></li>
            <li><span>08:30 - 09:10</span> <span>Sejarah</span></li>
            <li><span>09:25 - 10:45</span> <span>Bhs.Arab TL</span></li>
            <li><span>10:45 - 12:05</span> <span>Bhs.Inggris</span></li>
            <li><span>12:50 - 14:10</span> <span>Bhs.Jepang</span></li>
            <li><span>14:10 - 15:30</span> <span>Fiqih</span></li>
        </ul>

        <div class="day-schedule">Selasa</div>
        <ul class="subject-list">
            <li><span>07:10 - 09:10</span> <span>Matematika TL</span></li>
            <li><span>09:25 - 10:45</span> <span>PKN</span></li>
            <li><span>10:45 - 12:05</span> <span>Informatika</span></li>
            <li><span>12:50 - 14:10</span> <span>Alquran Hadist</span></li>
            <li><span>14:10 - 15:30</span> <span>SKI</span></li>
        </ul>
        <div class="day-schedule">Rabu</div>
        <ul class="subject-list">
            <li><span>07:10 - 08:30</span> <span>Seni Budaya</span></li>
            <li><span>08:30 - 09:10</span> <span>BK</span></li>
            <li><span>09:25 - 10:45</span> <span>Ekonomi</span></li>
            <li><span>10:45 - 12:05</span> <span>Bhs.Indonesia</span></li>
            <li><span>12:50 - 13:30</span> <span>Matematika Wajib</span></li>
            <li><span>13:30 - 15:00</span> <span>Pendidikan Jasmani</span></li>
        </ul>
        <div class="day-schedule">Kamis</div>
        <ul class="subject-list">
            <li><span>07:10 - 09:10</span> <span>Bhs.Inggris Wajib</span></li>
            <li><span>09:30 - 10:50</span> <span>Matematika Wajib</span></li>
            <li><span>10:50 - 12:00</span> <span>Bhs.Arab Wajib</span></li>
            <li><span>12:00 - 15:00</span> <span>Informatika</span></li>
        </ul>
        <div class="day-schedule">Jumat</div>
        <ul class="subject-list">
            <li><span>07:10 - 09:10</span> <span>Studi Riset</span></li>
            <li><span>09:30- 10:50</span> <span>PKWU</span></li>
            <li><span>10:50 - 11:30</span> <span>Tahfidz</span></li>
            <li><span>13:00- 15:00</span> <span>Ekonomi</span></li>
        </ul>
    </div>
</section>
<br>
<br>
<br>
<br>
<br>
    <!-- About Us -->
    <section id="about-us">
        <h2>About Us</h2>
        <p>Kami adalah kelas dengan semangat kebersamaan yang tinggi dan selalu mendukung satu sama lain. Di sini, kami percaya bahwa setiap anggota memiliki peran penting dalam perjalanan belajar bersama-sama.</p>
    </section>
    <br>
    <br>
    <br>
    <br>
    <br>

    <!-- Contact -->
    <section id="contact">
        <h2>Contact Us</h2>
        <p>Untuk informasi lebih lanjut, hubungi kami melalui email:</p>
        <p><strong>Email:</strong> kelas.example@example.com</p>
    </section>

    <footer>
        <p>© 2024 Kenangan Kelas</p>
    </footer>

    <script>
        let currentSlide = 0;
        const slides = document.querySelectorAll('.slideshow');

        function changeSlide(n) {
            slides[currentSlide].classList.remove('active');
            currentSlide = (currentSlide + n + slides.length) % slides.length;
            slides[currentSlide].classList.add('active');
        }
    </script>

</body>
</html>

