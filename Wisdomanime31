<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jay's Anime - Watch Your Favorite Anime</title>
    <!-- Google Fonts: Modern Font (Poppins) -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif; /* Modern font */
        }

        body {
            background-color: #1a1a1a;
            color: #fff;
            line-height: 1.6;
        }

        header {
            background: linear-gradient(90deg, #6a0dad, #2e0ca3); /* Purple Gradient */
            color: #fff;
            padding: 20px 0;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
        }

        header h1 {
            font-size: 2.2rem;
            margin-left: 30px;
            letter-spacing: 1.5px;
            font-weight: 600;
        }

        .menu {
            display: flex;
            gap: 25px;
            margin-right: 30px;
        }

        .menu a {
            text-decoration: none;
            color: #00ffff; /* Cyan */
            font-weight: 500;
            transition: color 0.3s ease;
        }

        .menu a:hover {
            color: #87ceeb; /* Sky Blue */
        }

        .hero {
            background: url('https://images.unsplash.com/photo-1615719427082-e8b5a5d3e2f8?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80') no-repeat center center/cover;
            height: 450px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #fff;
            text-align: center;
            position: relative;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5); /* Dark overlay */
        }

        .hero div {
            position: relative;
            z-index: 1;
        }

        .hero h2 {
            font-size: 3rem;
            margin-bottom: 20px;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5);
            font-weight: 600;
        }

        .hero p {
            font-size: 1.3rem;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.5);
            font-weight: 300;
        }

        .cta-button {
            display: inline-block;
            margin-top: 25px;
            padding: 12px 30px;
            background: #00ffff; /* Cyan */
            color: #000;
            text-decoration: none;
            border-radius: 6px;
            font-size: 1.1rem;
            font-weight: 500;
            transition: background 0.3s ease, transform 0.3s ease;
        }

        .cta-button:hover {
            background: #87ceeb; /* Sky Blue */
            transform: translateY(-3px);
        }

        .content {
            padding: 60px 20px;
            background: #1a1a1a;
        }

        .section-title {
            text-align: center;
            margin-bottom: 40px;
            font-size: 2.2rem;
            color: #00ffff; /* Cyan */
            text-transform: uppercase;
            letter-spacing: 2px;
            font-weight: 600;
        }

        .anime-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 25px;
        }

        .anime-card {
            background: #2b2b2b;
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            position: relative;
        }

        .anime-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.5);
        }

        .anime-card img {
            width: 100%;
            height: 250px;
            object-fit: cover;
        }

        .anime-card h3 {
            font-size: 1.3rem;
            margin: 20px;
            text-align: center;
            color: #00ffff; /* Cyan */
            text-transform: uppercase;
            letter-spacing: 1px;
            font-weight: 500;
        }

        .anime-card p {
            font-size: 0.95rem;
            color: #ccc;
            margin: 0 20px 20px;
            text-align: center;
            font-weight: 300;
        }

        .card-actions {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-bottom: 20px;
        }

        .card-actions button {
            padding: 10px 20px;
            border: none;
            border-radius: 6px;
            cursor: pointer;
            transition: background 0.3s ease, transform 0.3s ease;
            font-weight: 500;
        }

        .card-actions .play-btn {
            background: #00ffff; /* Cyan */
            color: #000;
        }

        .card-actions .download-btn {
            background: #6a0dad; /* Purple */
            color: #fff;
        }

        .card-actions button:hover {
            transform: translateY(-3px);
            opacity: 0.9;
        }

        .upload-section {
            background: #2b2b2b;
            margin: 60px auto;
            padding: 30px;
            max-width: 600px;
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
        }

        .upload-section h2 {
            font-size: 1.6rem;
            margin-bottom: 25px;
            color: #00ffff; /* Cyan */
            text-align: center;
            text-transform: uppercase;
            letter-spacing: 1px;
            font-weight: 600;
        }

        .upload-section input,
        .upload-section textarea,
        .upload-section button {
            display: block;
            width: 100%;
            margin-bottom: 20px;
            padding: 12px;
            border: none;
            border-radius: 6px;
            background: #333;
            color: #fff;
            font-weight: 300;
        }

        .upload-section button {
            background: #00ffff; /* Cyan */
            cursor: pointer;
            transition: background 0.3s ease, transform 0.3s ease;
            font-weight: 500;
        }

        .upload-section button:hover {
            background: #87ceeb; /* Sky Blue */
            transform: translateY(-3px);
        }

        footer {
            background: linear-gradient(90deg, #6a0dad, #2e0ca3); /* Purple Gradient */
            color: #fff;
            text-align: center;
            padding: 25px 0;
            box-shadow: 0 -4px 15px rgba(0, 0, 0, 0.3);
        }

        footer p {
            font-size: 0.95rem;
            margin-bottom: 10px;
            font-weight: 300;
        }

        footer a {
            color: #00ffff; /* Cyan */
            text-decoration: none;
            font-weight: 500;
        }

        footer a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <header>
        <h1>Jay's Anime</h1>
        <div class="menu">
            <a href="#home">Home</a>
            <a href="#movies">Movies</a>
            <a href="#all">All</a>
            <a href="#subbed">Subbed</a>
            <a href="#dubbed">Dubbed</a>
        </div>
    </header>

    <section class="hero" id="home">
        <div>
            <h2>Welcome to Jay's Anime</h2>
            <p>Discover and watch your favorite anime movies.</p>
            <a href="#all" class="cta-button">Explore Anime</a>
        </div>
    </section>

    <section class="content" id="all">
        <h2 class="section-title">Popular Anime</h2>
        <div class="anime-grid">
            <!-- Anime Card 1: Naruto -->
            <div class="anime-card">
                <img src="https://m.media-amazon.com/images/I/81QItsgaqNL._AC_UF1000,1000_QL80_.jpg" alt="Naruto">
                <h3>Naruto</h3>
                <p>A ninja's journey to become Hokage.</p>
                <div class="card-actions">
                    <button class="play-btn">Play</button>
                    <button class="download-btn">Download</button>
                </div>
            </div>

            <!-- Anime Card 2: One Piece -->
            <div class="anime-card">
                <img src="https://m.media-amazon.com/images/I/81vGmtKtWDL._AC_UF1000,1000_QL80_.jpg" alt="One Piece">
                <h3>One Piece</h3>
                <p>Pirates searching for the ultimate treasure.</p>
                <div class="card-actions">
                    <button class="play-btn">Play</button>
                    <button class="download-btn">Download</button>
                </div>
            </div>

            <!-- Anime Card 3: Attack on Titan -->
            <div class="anime-card">
                <img src="https://m.media-amazon.com/images/I/81rZwEzXxLL._AC_UF1000,1000_QL80_.jpg" alt="Attack on Titan">
                <h3>Attack on Titan</h3>
                <p>Humanity's fight against giant Titans.</p>
                <div class="card-actions">
                    <button class="play-btn">Play</button>
                    <button class="download-btn">Download</button>
                </div>
            </div>

            <!-- Anime Card 4: My Hero Academia -->
            <div class="anime-card">
                <img src="https://m.media-amazon.com/images/I/81kqRcCnTAL._AC_UF1000,1000_QL80_.jpg" alt="My Hero Academia">
                <h3>My Hero Academia</h3>
                <p>Young heroes training to save the world.</p>
                <div class="card-actions">
                    <button class="play-btn">Play</button>
                    <button class="download-btn">Download</button>
                </div>
            </div>

            <!-- Anime Card 5: Demon Slayer -->
            <div class="anime-card">
                <img src="https://m.media-amazon.com/images/I/81i+VZt1BUL._AC_UF1000,1000_QL80_.jpg" alt="Demon Slayer">
                <h3>Demon Slayer</h3>
                <p>A demon slayer's quest for vengeance.</p>
                <div class="card-actions">
                    <button class="play-btn">Play</button>
                    <button class="download-btn">Download</button>
                </div>
            </div>
        </div>
    </section>

    <section class="upload-section" id="upload">
        <h2>Upload Anime (Owner Only)</h2>
        <form>
            <input type="text" placeholder="Anime Title" required>
            <textarea placeholder="Description" rows="4" required></textarea>
            <input type="file" accept="video/*" required>
            <button type="submit">Upload Video</button>
        </form>
    </section>

    <footer>
        <p>Contact Us:</p>
        <p>Email: <a href="mailto:wisebrain2008@gmail.com">wisebrain2008@gmail.com</a></p>
        <p>&copy; 2023 Jay's Anime. All rights reserved.</p>
    </footer>
</body>
</html>
