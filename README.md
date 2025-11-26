<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Classify: Acids, Bases & Salts — Grade 11 Game</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header>
    <h1>Classify: Strong acids, Strong bases, Weak acids, Weak bases, Salts</h1>
    <p class="subtitle">Drag & drop or click to sort each term into one of the five boxes. Some terms are tricky — think about dissociation and common-ion behavior.</p>
  </header>

  <main>
    <section class="controls">
      <button id="shuffleBtn">Shuffle terms</button>
      <button id="resetBtn">Reset</button>
      <button id="checkBtn">Check answers</button>
      <button id="showKeyBtn">Show answer key</button>
      <div id="scoreBox">Score: <span id="score">0</span></div>
    </section>

    <section class="game">
      <div class="term-pool" aria-label="Term pool" id="termPool">
        <h2>Terms</h2>
        <div id="terms" class="terms-list" role="list"></div>
        <p class="hint">Tip: Click a term, then click a category to place it (useful on mobile).</p>
      </div>

      <div class="categories" id="categories">
        <div class="category" data-cat="Strong acid" id="cat-strong-acid" tabindex="0">
          <h3>Strong acids</h3>
          <div class="dropzone" data-cat="Strong acid"></div>
        </div>

        <div class="category" data-cat="Strong base" id="cat-strong-base" tabindex="0">
          <h3>Strong bases</h3>
          <div class="dropzone" data-cat="Strong base"></div>
        </div>

        <div class="category" data-cat="Weak acid" id="cat-weak-acid" tabindex="0">
          <h3>Weak acids</h3>
          <div class="dropzone" data-cat="Weak acid"></div>
        </div>

        <div class="category" data-cat="Weak base" id="cat-weak-base" tabindex="0">
          <h3>Weak bases</h3>
          <div class="dropzone" data-cat="Weak base"></div>
        </div>

        <div class="category" data-cat="Salt" id="cat-salt" tabindex="0">
          <h3>Salts</h3>
          <div class="dropzone" data-cat="Salt"></div>
        </div>
      </div>
    </section>

    <section class="explanation">
      <h2>Teacher notes (short)</h2>
      <ul>
        <li>Strong acids: complete (or near-complete) proton donors in aqueous solution (e.g., HCl, HNO3).</li>
        <li>Strong bases: soluble hydroxides of alkali metals and heavier alkaline earths (e.g., NaOH, KOH, Ba(OH)2).</li>
        <li>Weak acids/bases: partial dissociation (e.g., CH3COOH, NH3).</li>
        <li>Salts: ionic compounds formed from neutralization; some salts (NH4Cl, NaHSO4) show acidic or basic behavior in water — trick questions.</li>
      </ul>
    </section>

    <section class="feedback" id="feedback" aria-live="polite"></section>
  </main>

  <footer>
    <small>Designed for Grade 11 chemistry practice — includes intentional trick/decoy salts (e.g., NH4Cl, NaHSO4, KCN) to encourage thinking about hydrolysis and conjugate acid/base behavior.</small>
  </footer>

  <script src="app.js"></script>
</body>
</html>
