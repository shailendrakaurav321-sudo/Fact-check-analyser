!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Fact-Check Analyser</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header class="site-header">
    <h1>Fact-Check Analyser</h1>
    <p>Paste a claim, headline or article. Get a reliability check and the exact statements worth verifying.</p>
  </header>

  <main>
    <section class="panel" aria-labelledby="input-title">
      <h2 id="input-title">Text to analyse</h2>
      <label for="sourceUrl">Source link (optional)</label>
      <input type="url" id="sourceUrl" placeholder="https://example.com/article">

      <label for="inputText">Claim or article</label>
      <textarea id="inputText" rows="8" placeholder="Paste the text here..."></textarea>

      <div class="actions">
        <button id="analyseBtn" type="button">Analyse</button>
        <button id="sampleBtn" type="button" class="secondary">Try a sample</button>
        <button id="clearBtn" type="button" class="secondary">Clear</button>
      </div>
      <p id="error" class="error" role="alert" hidden></p>
    </section>

    <section id="results" class="panel" hidden aria-live="polite">
      <h2>Result</h2>

      <div class="score-row">
        <div id="scoreCircle" class="score-circle"><span id="scoreValue">0</span></div>
        <div>
          <p id="verdict" class="verdict"></p>
          <p class="note">This score measures how the text is written, not whether it is true.</p>
        </div>
      </div>

      <h3>Warning signs found</h3>
      <ul id="flagList" class="list"></ul>

      <h3>Claims to verify</h3>
      <ol id="claimList" class="list"></ol>

      <h3>Check it yourself</h3>
      <div id="links" class="links"></div>
    </section>
  </main>

  <footer>
    <p>An automated check cannot confirm facts. Always compare with trusted sources.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html># Fact-check-analyser
Fact check analyser 
