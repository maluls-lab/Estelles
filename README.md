<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Spotify</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: #191414;
            color: #fff;
            font-family: Arial, sans-serif;
            display: flex;
            height: 100vh;
        }

        /* Sidebar */
        .sidebar {
            width: 250px;
            background: #121212;
            padding: 20px;
            overflow-y: auto;
            border-right: 1px solid #282828;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            color: #1DB954;
            margin-bottom: 30px;
        }

        .nav-item {
            padding: 12px;
            margin: 10px 0;
            cursor: pointer;
            border-radius: 8px;
            transition: 0.3s;
        }

        .nav-item:hover {
            background: #282828;
        }

        /* Main Content */
        .main {
            flex: 1;
            display: flex;
            flex-direction: column;
        }

        .header {
            background: #1DB954;
            padding: 20px;
            text-align: center;
        }

        .content {
            flex: 1;
            padding: 20px;
            overflow-y: auto;
        }

        .playlist-title {
            font-size: 28px;
            margin-bottom: 20px;
        }

        .musicas {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
            gap: 15px;
        }

        .musica-card {
            background: #282828;
            padding: 15px;
            border-radius: 8px;
            cursor: pointer;
            transition: 0.3s;
            text-align: center;
        }

        .musica-card:hover {
            background: #1DB954;
            transform: scale(1.05);
        }

        .musica-img {
            width: 100%;
            height: 120px;
            background: #1DB954;
            border-radius: 8px;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 40px;
        }

        .musica-nome {
            font-weight: bold;
            margin-bottom: 5px;
        }

        .musica-artista {
            font-size: 12px;
            color: #b3b3b3;
        }

        /* Player */
        .player {
            background: #181818;
            padding: 15px;
            border-top: 1px solid #282828;
            text-align: center;
        }

        .player-info {
            margin-bottom: 10px;
            font-size: 12px;
        }
    </style>
</head>
<body>
    <!-- Sidebar -->
    <div class="sidebar">
        <div class="logo">🎵 Spotify</div>
        <div class="nav-item">🏠 Home</div>
        <div class="nav-item">🔍 Buscar</div>
        <div class="nav-item">📚 Sua Biblioteca</div>
        <div class="nav-item">❤️ Músicas Marcadas</div>
        <div class="nav-item">🎧 Podcasts</div>
    </div>

    <!-- Main Content -->
    <div class="main">
        <div class="header">
            <h1>Minha Playlist</h1>
        </div>

        <div class="content">
            <h2 class="playlist-title">Músicas Favoritas</h2>
            <div class="musicas">
                <div class="musica-card">
                    <div class="musica-img">🎵</div>
                    <div class="musica-nome">Bohemian</div>
                    <div class="musica-artista">Queen</div>
                </div>
                <div class="musica-card">
                    <div class="musica-img">🎸</div>
                    <div class="musica-nome">Stairway</div>
                    <div class="musica-artista">Led Zeppelin</div>
                </div>
                <div class="musica-card">
                    <div class="musica-img">🎹</div>
                    <div class="musica-nome">Imagine</div>
                    <div class="musica-artista">John Lennon</div>
                </div>
                <div class="musica-card">
                    <div class="musica-img">🎤</div>
                    <div class="musica-nome">Hallelujah</div>
                    <div class="musica-artista">Leonard Cohen</div>
                </div>
            </div>
        </div>

        <div class="player">
            <div class="player-info">▶️ Bohemian - Queen | 2:43</div>
            <div style="background: #404040; height: 5px; border-radius: 5px;">
                <div style="background: #1DB954; height: 100%; width: 40%; border-radius: 5px;"></div>
            </div>
        </div>
    </div>
</body>
</html>
