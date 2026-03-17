<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content=
"width=device-width, initial-scale=1.0"
>
    <title>WATCHDOG | Full Investigation</title>
    <style>
        /* CSS Palette: Blue #003366 | Yellow #FFD700 | White #FFFFFF */
        :root {
            --blue: #003366;
            --yellow: #FFD700;
            --white: #FFFFFF;
            --grey: #f4f4f4;
        }

        body { font-family: 'Georgia', serif; line-height: 1.8; margin: 0; background: var(--white); color: #222; }

        /* Reading Progress Bar */
        #progress-container { position: fixed; top: 0; width: 100%; height: 5px; background: transparent; z-index: 2000; }
        #progress-bar { height: 100%; background: var(--yellow); width: 0%; }

        /* Nav */
        .watchdog-nav {
            background-color: var(--blue);
            color: white;
            padding: 15px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 5px solid var(--yellow);
        }
        .logo { font-size: 24px; font-weight: bold; color: var(--yellow); text-decoration: none; font-family: sans-serif; }
        .watchdog-nav a { color: white; text-decoration: none; margin-left: 20px; font-weight: bold; font-family: sans-serif; }

        /* Article Layout */
        .article-header { background: var(--grey); padding: 60px 10%; border-bottom: 1px solid #ddd; }
        .category-tag { background: var(--yellow); color: var(--blue); padding: 5px 10px; font-weight: bold; font-family: sans-serif; text-transform: uppercase; font-size: 12px; }
        h1 { font-size: 48px; color: var(--blue); margin: 20px 0; line-height: 1.1; }
        
        .article-container { max-width: 800px; margin: 40px auto; padding: 0 20px; }
        .evidence-box { background: #fffde7; border: 2px dashed var(--blue); padding: 20px; margin: 30px 0; display: none; }
        
        /* Interactive Button */
        .btn-reveal {
            background: var(--blue);
            color: white;
            padding: 15px 30px;
            border: none;
            cursor: pointer;
            font-weight: bold;
            font-family: sans-serif;
            display: block;
            margin: 20px 0;
        }
        .btn-reveal:hover { background: #0056b3; }

        footer { background: var(--blue); color: white; padding: 40px; text-align: center; margin-top: 60px; }
    </style>
</head>
<body>

    <div id="progress-container"><div id="progress-bar"></div></div>

    <nav class="watchdog-nav">
        <a href="index.html" class="logo">WATCHDOGORG</a>
        <div>
            <a href="index.html">Latest</a>
            <a href="investigations.html">Investigations</a>
        </div>
    </nav>

    <header class="article-header">
        <span class="category-tag">Investigative Report</span>
        <h1>The Local Investigation: How non profit organizations are laundering money in nowadays</h1>
        <p><strong>By Watchdog Staff</strong></p>
        <p2>Published March 17, 2026 </p2>
    </header>

    <main class="article-container">
        <p>For months, Watchdog investigators have been tracking non profit organizations in Los Angeles</p>
        
        <p>Till our investigation due to Weighart house is ongoing, we publish evidence of another huge case </p>

        <button class="btn-reveal" onclick="toggleEvidence()">REVEAL CONFIDENTIAL DATA</button>
        
        <div>
    <h2>INTERNAL DATA LOG: CASE #2026-NPO</h2>
    <p>Evidence gathered from U.S. Department of Justice and LA County District Attorney filings:</p>
    <ul>
        <li><strong>Abundant Blessings:</strong> $23M diverted from homeless services to luxury real estate and private jets.</li>
        <li><strong>The Painted Turtle:</strong> $5.2M embezzled from medical camp funds.</li>
        <li><strong>Red Flag:</strong> Use of "ghost" board members and fabricated vendor invoices.</li>
    </ul>
</div>

        <p>This investigation continues. We are now looking into car rental agencies and searching evidence of sales of stolen cars</p>
    </main>

    <footer>
        <p>&copy; 2026 WATCHDOG | Truth in Local Reporting</p>
    </footer>

    <script>
        // Dynamics: Reading Progress Bar
        window.onscroll = function() {
            let winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            let height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            let scrolled = (winScroll / height) * 100;
            document.getElementById("progress-bar").style.width = scrolled + "%";
        };

        // Dynamics: Toggle Evidence Box
        function toggleEvidence() {
            let box = document.getElementById('evidence');
            if (box.style.display === "none" || box.style.display === "") {
                box.style.display = "block";
                alert("Accessing Secure Case Files...");
            } else {
                box.style.display = "none";
            }
        }
    </script>
</body>
</html>

