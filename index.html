<!DOCTYPE html>
<html lang="sw">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Historia ya Nchi Duniani</title>
    <style>
        /* CSS YA KUREMBA WEBSITE */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f2f5;
            color: #333;
        }

        header {
            background-color: #1a2a6c;
            color: white;
            padding: 40px 20px;
            text-align: center;
            box-shadow: 0 4px 10px rgba(0,0,0,0.2);
        }

        h1 { margin: 0; font-size: 2.5rem; }
        p.subtitle { margin-top: 10px; opacity: 0.8; }

        .search-container {
            margin: -25px auto 30px;
            max-width: 600px;
            display: flex;
            gap: 10px;
            padding: 0 20px;
        }

        input {
            flex: 1;
            padding: 15px;
            border: none;
            border-radius: 30px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            font-size: 16px;
            outline: none;
        }

        button {
            padding: 15px 30px;
            border: none;
            background-color: #f2994a;
            color: white;
            font-weight: bold;
            border-radius: 30px;
            cursor: pointer;
            transition: 0.3s;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }

        button:hover { background-color: #e67e22; transform: translateY(-2px); }

        main {
            max-width: 900px;
            margin: 0 auto 50px;
            padding: 20px;
        }

        .card {
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.05);
            display: none; /* Inafichwa mpaka itafutwe */
        }

        .country-header {
            display: flex;
            align-items: center;
            gap: 20px;
            border-bottom: 2px solid #eee;
            padding-bottom: 20px;
            margin-bottom: 20px;
        }

        .country-header img {
            width: 120px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .history-text {
            line-height: 1.8;
            font-size: 18px;
            text-align: justify;
        }

        .loading { text-align: center; display: none; font-style: italic; color: #666; }
        
        .footer { text-align: center; padding: 20px; font-size: 14px; color: #777; }
    </style>
</head>
<body>

    <header>
        <h1>Maktaba ya Historia</h1>
        <p class="subtitle">Gundua chimbuko na matukio muhimu ya kila nchi duniani</p>
    </header>

    <div class="search-container">
        <input type="text" id="countrySearch" placeholder="Andika nchi (mfano: Tanzania, Germany, Japan)..." onkeypress="handleKeyPress(event)">
        <button onclick="searchHistory()">Tafuta</button>
    </div>

    <main>
        <div id="loading" class="loading">Inatafuta taarifa, tafadhali subiri...</div>
        
        <div id="resultCard" class="card">
            <div class="country-header">
                <img id="flagImg" src="" alt="Bendera">
                <h2 id="countryName">Jina la Nchi</h2>
            </div>
            <div id="historyContent" class="history-text">
                </div>
            <div style="margin-top: 25px;">
                <a id="wikiLink" href="#" target="_blank" style="color: #1a2a6c; font-weight: bold; text-decoration: none;">&rarr; Soma historia kamili Wikipedia</a>
            </div>
        </div>
    </main>

    <div class="footer">
        &copy; 2024 Tovuti ya Historia ya Dunia | Imetengenezwa kwa ajili yako.
    </div>

    <script>
        // JAVASCRIPT YA KUTAFUTA DATA
        async function searchHistory() {
            const query = document.getElementById('countrySearch').value.trim();
            const resultCard = document.getElementById('resultCard');
            const loading = document.getElementById('loading');

            if (!query) {
                alert("Tafadhali andika jina la nchi!");
                return;
            }

            // Onyesha loading, ficha matokeo ya zamani
            loading.style.display = "block";
            resultCard.style.display = "none";

            try {
                // Tunatumia Wikipedia API kupata muhtasari (Summary)
                const response = await fetch(`https://en.wikipedia.org/api/rest_v1/page/summary/${query}`);
                const data = await response.json();

                if (data.title === "Not found" || data.type === "disambiguation") {
                    loading.innerHTML = "❌ Hatukuweza kupata historia ya nchi hiyo. Jaribu kuandika kwa Kiingereza.";
                } else {
                    // Jaza data kwenye page
                    document.getElementById('countryName').innerText = data.title;
                    document.getElementById('historyContent').innerText = data.extract;
                    document.getElementById('wikiLink').href = data.content_urls.desktop.page;
                    
                    if (data.thumbnail) {
                        document.getElementById('flagImg').src = data.thumbnail.source;
                        document.getElementById('flagImg').style.display = "block";
                    } else {
                        document.getElementById('flagImg').style.display = "none";
                    }

                    // Onyesha kadi ya matokeo
                    loading.style.display = "none";
                    resultCard.style.display = "block";
                }
            } catch (error) {
                loading.innerHTML = "❌ Hitilafu ya mtandao imetokea.";
                console.error(error);
            }
        }

        // Ruhusu kubonyeza 'Enter' kutafuta
        function handleKeyPress(e) {
            if (e.keyCode === 13) {
                searchHistory();
            }
        }
    </script>

</body>
</html>
