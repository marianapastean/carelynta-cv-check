<!DOCTYPE html>
<html lang="ro">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
  <meta name="theme-color" content="#0a3258">
  <meta name="description" content="CARELYNTA CV CHECK – verifică gratuit structura CV-ului și descoperă ce poți îmbunătăți.">
  <meta http-equiv="Cache-Control" content="no-cache, no-store, must-revalidate">
  <title>CARELYNTA CV CHECK | Verificare gratuită CV</title>

  <style>
    :root {
      --primary: #0a3258;
      --primary-dark: #062441;
      --deep: #061d35;
      --gold: #c6a66a;
      --gold-light: #dfc18a;
      --text: #263442;
      --muted: #687887;
      --background: #f3f6f9;
      --white: #ffffff;
      --soft: #e9f0f7;
      --border: #d8e2ec;
      --success: #247653;
      --warning: #98691d;
      --shadow: 0 12px 32px rgba(10,50,88,.08);
    }

    * {
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
      -webkit-text-size-adjust: 100%;
      text-size-adjust: 100%;
    }

    body {
      margin: 0;
      font-family: Arial, Helvetica, sans-serif;
      color: var(--text);
      background: var(--background);
      line-height: 1.6;
      overflow-x: hidden;
    }

    img {
      max-width: 100%;
    }

    button,
    textarea,
    input {
      font: inherit;
    }

    .container {
      width: min(100% - 36px, 1000px);
      margin: 0 auto;
    }

    .topbar {
      background: var(--deep);
      color: white;
      text-align: center;
      padding: 10px 14px;
      font-size: 11px;
      letter-spacing: 1.5px;
      border-bottom: 3px solid var(--gold);
    }

    header {
      text-align: center;
      padding: 42px 15px 32px;
    }

    .logo {
      display: block;
      width: 145px;
      height: 115px;
      object-fit: contain;
      margin: 0 auto 10px;
    }

    .brand {
      color: var(--primary);
      font-weight: bold;
      letter-spacing: 5px;
      font-size: 15px;
      margin: 0 0 15px;
    }

    .eyebrow {
      display: inline-block;
      background: var(--soft);
      color: var(--primary);
      border: 1px solid var(--border);
      padding: 7px 15px;
      border-radius: 30px;
      font-size: 11px;
      font-weight: bold;
      letter-spacing: 1px;
      text-transform: uppercase;
    }

    h1 {
      color: var(--primary);
      font-size: clamp(38px, 6vw, 60px);
      line-height: 1.1;
      margin: 18px 0 15px;
      letter-spacing: -2px;
    }

    .lead {
      max-width: 700px;
      margin: 0 auto;
      color: var(--muted);
      font-size: 17px;
    }

    .lead strong {
      color: var(--primary);
    }

    .trust {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 10px 24px;
      margin-top: 22px;
      color: var(--muted);
      font-size: 13px;
    }

    .trust span::before {
      content: "✓ ";
      color: var(--primary);
      font-weight: bold;
    }

    .panel {
      background: var(--white);
      border: 1px solid var(--border);
      border-radius: 22px;
      padding: clamp(20px, 4vw, 36px);
      margin: 22px 0;
      box-shadow: var(--shadow);
      min-width: 0;
    }

    .kicker {
      color: var(--primary);
      font-size: 11px;
      font-weight: bold;
      letter-spacing: 2px;
      text-transform: uppercase;
      margin: 0 0 7px;
    }

    h2 {
      color: var(--primary);
      font-size: clamp(22px, 4vw, 27px);
      line-height: 1.25;
      margin: 0 0 10px;
      overflow-wrap: anywhere;
    }

    .hint {
      color: var(--muted);
      font-size: 14px;
      margin: 0 0 20px;
    }

    label {
      display: block;
      color: var(--primary);
      font-weight: bold;
      font-size: 14px;
      margin: 20px 0 8px;
    }

    .optional {
      color: var(--muted);
      font-weight: normal;
    }

    textarea {
      display: block;
      width: 100%;
      min-height: 210px;
      padding: 15px;
      border: 1px solid #cbd6e0;
      border-radius: 13px;
      outline: none;
      background: white;
      color: var(--text);
      font-family: Arial, Helvetica, sans-serif;
      font-size: 16px;
      line-height: 1.6;
      resize: vertical;
      -webkit-appearance: none;
      appearance: none;
    }

    textarea::placeholder {
      color: #9aa8b5;
    }

    textarea:focus {
      border-color: var(--primary);
      box-shadow: 0 0 0 4px rgba(10,50,88,.12);
    }

    #job {
      min-height: 135px;
    }

    .upload-section {
      margin: 20px 0 25px;
    }

    .upload-title {
      display: block;
      color: var(--primary);
      font-weight: bold;
      font-size: 14px;
      margin-bottom: 10px;
    }

    .upload-box {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      gap: 9px;
      padding: 26px 16px;
      border: 2px dashed var(--primary);
      border-radius: 16px;
      background: var(--soft);
      cursor: pointer;
      text-align: center;
      margin: 0;
      width: 100%;
    }

    .upload-icon {
      font-size: 32px;
    }

    .upload-box strong {
      color: var(--primary);
      font-size: 16px;
    }

    .upload-box span {
      color: var(--muted);
      font-size: 13px;
      overflow-wrap: anywhere;
    }

    .upload-box .upload-button {
      display: inline-block;
      background: var(--primary);
      color: white;
      padding: 10px 22px;
      border-radius: 25px;
      font-weight: bold;
      margin-top: 5px;
    }

    .file-input {
      position: absolute;
      width: 1px;
      height: 1px;
      opacity: 0;
      pointer-events: none;
    }

    .file-input:focus-visible + .upload-box {
      outline: 3px solid var(--gold);
      outline-offset: 4px;
    }

    .file-status {
      margin: 12px 0 0;
      color: var(--primary);
      font-size: 13px;
      font-weight: bold;
      overflow-wrap: anywhere;
    }

    .upload-note {
      color: var(--muted);
      font-size: 12px;
      line-height: 1.5;
      margin-top: 7px;
    }

    .actions {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
      margin-top: 20px;
    }

    button {
      border: none;
      border-radius: 50px;
      padding: 14px 24px;
      min-height: 48px;
      background: var(--primary);
      color: white;
      font-size: 15px;
      font-weight: bold;
      cursor: pointer;
      transition: background .2s ease;
      -webkit-appearance: none;
      appearance: none;
      touch-action: manipulation;
    }

    button:hover {
      background: var(--primary-dark);
    }

    button.secondary {
      background: var(--soft);
      color: var(--primary);
    }

    button.secondary:hover {
      background: #dce8f3;
    }

    button:focus-visible {
      outline: 3px solid var(--gold);
      outline-offset: 3px;
    }

    button:disabled {
      opacity: .65;
      cursor: wait;
    }

    .privacy {
      color: var(--muted);
      font-size: 12px;
      margin-top: 16px;
    }

    .hidden {
      display: none !important;
    }

    .results-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      gap: 15px;
    }

    .score {
      color: var(--primary);
      font-size: 44px;
      font-weight: 900;
      white-space: nowrap;
    }

    .score small {
      font-size: 15px;
      color: var(--muted);
    }

    .meter {
      height: 11px;
      background: #e7edf3;
      border-radius: 30px;
      overflow: hidden;
      margin: 15px 0 20px;
    }

    .meter span {
      display: block;
      height: 100%;
      width: 0;
      background: linear-gradient(90deg, var(--primary), #7898b6);
      border-radius: 30px;
      transition: width .4s;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 13px;
    }

    .item {
      background: #f8fafc;
      border: 1px solid var(--border);
      border-radius: 14px;
      padding: 16px;
      min-width: 0;
      overflow-wrap: anywhere;
    }

    .item strong {
      display: block;
      color: var(--primary);
      margin-bottom: 6px;
    }

    .status {
      color: var(--success);
      font-size: 11px;
      font-weight: bold;
      text-transform: uppercase;
    }

    .status.warn {
      color: var(--warning);
    }

    .item p {
      color: var(--muted);
      font-size: 13px;
      margin: 6px 0 0;
    }

    .keyword-section {
      margin-top: 25px;
      padding-top: 22px;
      border-top: 1px solid var(--border);
      overflow-wrap: anywhere;
    }

    .keyword-section h3 {
      color: var(--primary);
      margin: 0 0 8px;
    }

    .keyword-section p {
      color: var(--muted);
      font-size: 13px;
    }

    .tag {
      display: inline-block;
      background: var(--soft);
      color: var(--primary);
      padding: 6px 10px;
      border-radius: 20px;
      font-size: 12px;
      margin: 4px;
      overflow-wrap: anywhere;
    }

    .cta {
      margin-top: 28px;
      padding: 30px;
      border-radius: 18px;
      background: linear-gradient(135deg, var(--primary), var(--deep));
      color: white;
      border: 1px solid rgba(198,166,106,.45);
      overflow-wrap: anywhere;
    }

    .cta .kicker {
      color: var(--gold-light);
    }

    .cta h2 {
      color: white;
      font-size: 25px;
      margin-bottom: 15px;
    }

    .cta p {
      color: #e0e8ef;
      font-size: 14px;
      line-height: 1.75;
    }

    .cta p strong {
      color: white;
    }

    .cta a.cta-button {
      display: inline-block;
      margin-top: 12px;
      padding: 15px 24px;
      border-radius: 50px;
      background: var(--gold);
      color: var(--deep);
      font-size: 15px;
      font-weight: bold;
      text-decoration: none;
      text-align: center;
      max-width: 100%;
    }

    .how-grid {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 14px;
      margin: 25px 0;
    }

    .how-card {
      background: white;
      border: 1px solid var(--border);
      border-radius: 16px;
      padding: 20px;
      min-width: 0;
    }

    .number {
      display: grid;
      place-items: center;
      width: 32px;
      height: 32px;
      background: var(--primary);
      color: white;
      border-radius: 50%;
      font-weight: bold;
      margin-bottom: 12px;
    }

    .how-card strong {
      color: var(--primary);
      display: block;
    }

    .how-card p {
      color: var(--muted);
      font-size: 13px;
      margin-bottom: 0;
    }

    footer {
      text-align: center;
      padding: 28px 10px 40px;
      color: var(--muted);
      font-size: 12px;
    }

    footer strong {
      color: var(--primary);
      letter-spacing: 3px;
    }

    /* OPTIMIZARE TABLETĂ */
    @media (max-width: 800px) {
      .container {
        width: min(100% - 28px, 1000px);
      }

      .how-grid {
        grid-template-columns: 1fr 1fr;
      }
    }

    /* OPTIMIZARE TELEFOANE */
    @media (max-width: 600px) {
      .container {
        width: calc(100% - 24px);
      }

      .topbar {
        font-size: 9px;
        letter-spacing: 1px;
        padding: 9px 8px;
      }

      header {
        padding: 26px 5px 22px;
      }

      .logo {
        width: 112px;
        height: 90px;
      }

      .brand {
        font-size: 14px;
        letter-spacing: 4px;
      }

      .eyebrow {
        font-size: 10px;
        padding: 7px 12px;
      }

      h1 {
        font-size: 42px;
        letter-spacing: -1.5px;
      }

      .lead {
        font-size: 15px;
        line-height: 1.6;
      }

      .trust {
        gap: 8px 15px;
        font-size: 12px;
      }

      .panel {
        padding: 19px 16px;
        margin: 16px 0;
        border-radius: 17px;
      }

      h2 {
        font-size: 23px;
      }

      .hint {
        font-size: 13px;
      }

      textarea {
        min-height: 185px;
        padding: 13px;
        font-size: 16px;
      }

      #job {
        min-height: 125px;
      }

      .upload-box {
        padding: 22px 12px;
      }

      .actions {
        flex-direction: column;
        gap: 10px;
      }

      .actions button {
        width: 100%;
        min-height: 50px;
      }

      .results-header {
        align-items: flex-start;
      }

      .score {
        font-size: 38px;
      }

      .grid,
      .how-grid {
        grid-template-columns: 1fr;
      }

      .item {
        padding: 15px;
      }

      .cta {
        padding: 22px 17px;
      }

      .cta h2 {
        font-size: 22px;
      }

      .cta a.cta-button {
        display: block;
        width: 100%;
        padding: 15px 12px;
        font-size: 14px;
      }

      footer {
        padding-bottom: 30px;
      }
    }

    /* TELEFOANE FOARTE ÎNGUSTE */
    @media (max-width: 360px) {
      .container {
        width: calc(100% - 18px);
      }

      .panel {
        padding: 16px 13px;
      }

      h1 {
        font-size: 37px;
      }

      .score {
        font-size: 34px;
      }
    }

    /* PDF */
    .pdf-generating {
      background: #ffffff !important;
      color: #263442 !important;
      box-shadow: none !important;
    }

    .pdf-generating .actions {
      display: none !important;
    }

    .pdf-generating .item {
      break-inside: avoid;
      page-break-inside: avoid;
    }

    @media print {
      body {
        background: white;
      }

      .pdf-generating {
        width: 100%;
      }
    }
  </style>
</head>

<body>
  <div class="topbar">
    CAREER COACHING · CV OPTIMIZATION · PROFESSIONAL DEVELOPMENT
  </div>

  <main class="container">

    <header>
      <img
        class="logo"
        src="Logo%20Carelynta%20(2).png"
        alt="Logo CARELYNTA"
        onerror="this.style.display='none'"
      >

      <p class="brand">CARELYNTA</p>
      <span class="eyebrow">Instrument gratuit de verificare</span>

      <h1>CV CHECK</h1>

      <p class="lead">
        <strong>CV-ul tău merită să fie remarcat.</strong>
        CARELYNTA CV CHECK este un instrument gratuit care te ajută
        să verifici structura și conținutul CV-ului tău.
        Identifică punctele forte și descoperă ce poți îmbunătăți
        pentru a-ți prezenta experiența profesională mai clar
        și mai convingător.
        Primul pas către următoarea oportunitate profesională începe aici.
      </p>

      <div class="trust">
        <span>Gratuit</span>
        <span>Rapid</span>
        <span>Confidențial</span>
      </div>
    </header>

    <section class="panel input-panel">
      <p class="kicker">Primul pas către următoarea oportunitate</p>
      <h2>Verifică CV-ul tău</h2>

      <p class="hint">
        Încarcă documentul CV în format PDF sau Word ori copiază
        manual textul în câmpul de mai jos. Opțional, adaugă
        anunțul de angajare pentru o comparație orientativă.
      </p>

      <div class="upload-section">
        <span class="upload-title">Încarcă CV-ul tău</span>

        <input
          type="file"
          id="cvFile"
          class="file-input"
          accept=".pdf,.docx,application/pdf,application/vnd.openxmlformats-officedocument.wordprocessingml.document"
        >

        <label class="upload-box" for="cvFile">
          <span class="upload-icon">📄</span>
          <strong>Alege documentul CV</strong>
          <span>Formate acceptate: PDF și Word (.docx)</span>
          <span class="upload-button">Selectează fișierul</span>
        </label>

        <p id="fileStatus" class="file-status" aria-live="polite">
          Nu ai selectat încă un document.
        </p>

        <p class="upload-note">
          Documentul este procesat local în browser. Nu este trimis
          către un server CARELYNTA. Documentele PDF scanate ca imagini
          necesită recunoaștere optică a textului (OCR).
        </p>
      </div>

      <label for="cv">Sau copiază manual textul CV-ului</label>
      <textarea
        id="cv"
        placeholder="Copiază aici conținutul CV-ului: date de contact, profil profesional, experiență, educație, competențe etc."
      ></textarea>

      <label for="job">
        Anunțul de angajare
        <span class="optional">(opțional)</span>
      </label>

      <textarea
        id="job"
        placeholder="Copiază aici descrierea jobului pentru care aplici."
      ></textarea>

      <div class="actions">
        <button id="check" type="button">Verifică CV-ul gratuit</button>
        <button id="clear" class="secondary" type="button">Șterge textul</button>
      </div>

      <p class="privacy">
        Confidențialitate: analiza și extragerea textului se efectuează
        local, în browser. Documentul și textul introdus nu sunt trimise
        către CARELYNTA și nu sunt salvate de acest instrument.
      </p>
    </section>

    <section class="panel hidden" id="results" aria-live="polite">
      <div class="results-header">
        <div>
          <p class="kicker">Rezultatul verificării</p>
          <h2>Raportul tău CARELYNTA</h2>
          <p class="hint">Scor orientativ bazat pe criteriile de mai jos.</p>
        </div>

        <div class="score" id="score">0<small> / 100</small></div>
      </div>

      <div class="meter">
        <span id="bar"></span>
      </div>

      <p class="hint" id="score-description"></p>
      <div class="grid" id="checks"></div>

      <div class="keyword-section hidden" id="keywords">
        <h3>Potrivirea cu anunțul de angajare</h3>
        <p>
          Comparație orientativă a termenilor din anunț cu textul
          introdus în CV. Verifică manual relevanța fiecărui termen.
        </p>
        <div id="keyword-list"></div>
      </div>

      <div class="cta">
        <p class="kicker">Următorul pas în cariera ta</p>

        <h2>Un CV bun îți poate deschide ușa către o nouă oportunitate.</h2>

        <p>
          Ai făcut primul pas verificându-ți CV-ul.
          Acum este momentul să te asiguri că experiența,
          competențele și realizările tale sunt prezentate
          într-un mod profesionist și convingător.
        </p>

        <p>
          Prin serviciile CARELYNTA de consiliere în carieră
          și optimizare CV, te pot ajuta să îți clarifici
          direcția profesională, să îți evidențiezi punctele
          forte și să îți pregătești candidatura pentru
          oportunitățile pe care ți le dorești.
        </p>

        <p>
          <strong>
            Experiența ta merită să fie pusă în valoare.
            Hai să lucrăm împreună la următorul tău pas profesional!
          </strong>
        </p>

        <a
          class="cta-button"
          href="mailto:mariana.pastean@gmail.com?subject=Solicitare%20consiliere%20si%20optimizare%20CV&body=Buna%2C%20Mariana!%0A%0ADoresc%20sa%20aflu%20mai%20multe%20despre%20serviciile%20CARELYNTA%20de%20consiliere%20in%20cariera%20si%20optimizare%20CV.%0A%0AMultumesc!"
        >
          Hai să discutăm despre CV-ul meu →
        </a>
      </div>

      <p class="privacy">
        Acest raport este orientativ. Nu reprezintă o evaluare ATS reală
        și nu garantează obținerea unui interviu sau angajarea.
      </p>

      <div class="actions" data-html2canvas-ignore="true">
        <button id="print" class="secondary" type="button">
          Salvează raportul ca PDF
        </button>
      </div>
    </section>

    <section class="how-grid">
      <article class="how-card">
        <span class="number">1</span>
        <strong>Încarcă sau introdu CV-ul</strong>
        <p>Încarcă un PDF sau DOCX ori copiază manual textul CV-ului.</p>
      </article>

      <article class="how-card">
        <span class="number">2</span>
        <strong>Adaugă anunțul de angajare</strong>
        <p>Compară termenii din CV cu cerințele rolului.</p>
      </article>

      <article class="how-card">
        <span class="number">3</span>
        <strong>Analizează recomandările</strong>
        <p>Descoperă ce poți îmbunătăți în CV-ul tău.</p>
      </article>
    </section>

    <footer>
      <strong>CARELYNTA</strong>
      <div>CV CHECK · Instrument gratuit de orientare profesională</div>
      <div>© <span id="year"></span> CARELYNTA. Toate drepturile rezervate.</div>
    </footer>

  </main>

  <!-- Biblioteci pentru citirea documentelor și generarea PDF -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/pdf.js/3.11.174/pdf.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/mammoth/1.8.0/mammoth.browser.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.10.1/html2pdf.bundle.min.js"></script>

  <script>
    "use strict";

    const $ = id => document.getElementById(id);

    $("year").textContent = new Date().getFullYear();

    /* CONFIGURARE PDF.JS */
    if (window.pdfjsLib) {
      pdfjsLib.GlobalWorkerOptions.workerSrc =
        "https://cdnjs.cloudflare.com/ajax/libs/pdf.js/3.11.174/pdf.worker.min.js";
    }

    /* CRITERII DE VERIFICARE */
    const checks = [
      {
        name: "Date de contact",
        test: t => /e-?mail|@|(\+?\d[\d\s().-]{7,}\d)/i.test(t),
        good: "Am identificat indicii de e-mail sau număr de telefon.",
        bad: "Adaugă o adresă de e-mail profesională și un număr de telefon."
      },
      {
        name: "Profil profesional",
        test: t => /(profil profesional|despre mine|sumar profesional|obiectiv profesional|rezumat profesional)/i.test(t),
        good: "Există o secțiune de prezentare profesională.",
        bad: "Adaugă un rezumat de 3–5 rânduri despre experiență, competențe și obiective."
      },
      {
        name: "Experiență profesională",
        test: t => /(experiență profesională|experienta profesionala|experiență|experienta|work experience)/i.test(t),
        good: "Am identificat o secțiune de experiență.",
        bad: "Include rolul, angajatorul, perioada și responsabilitățile relevante."
      },
      {
        name: "Educație și formare",
        test: t => /(educație|educatie|studii|formare|universitate|liceu|cursuri)/i.test(t),
        good: "Am identificat informații despre educație sau formare.",
        bad: "Adaugă studiile, cursurile și certificările relevante."
      },
      {
        name: "Competențe",
        test: t => /(competențe|competente|abilități|abilitati|skills)/i.test(t),
        good: "Există o secțiune dedicată competențelor.",
        bad: "Include competențe tehnice și transferabile relevante pentru rol."
      },
      {
        name: "Structură cu titluri clare",
        test: t =>
          /(experiență|experienta|educație|educatie|competențe|competente)/i.test(t) &&
          /(profil|contact|limbi|certificări|certificari|studii)/i.test(t),
        good: "Apar mai multe titluri uzuale de secțiuni.",
        bad: "Folosește titluri standard: Profil, Experiență, Educație și Competențe."
      },
      {
        name: "Realizări și rezultate",
        test: t => /(realizări|realizari|rezultate|%|majorat|redus|crescut|implementat|optimizat|gestionat|îmbunătățit|imbunatatit)/i.test(t),
        good: "Am identificat indicii de rezultate sau contribuții.",
        bad: "Adaugă realizări concrete și rezultate măsurabile, unde este posibil."
      },
      {
        name: "Lungime și detaliu",
        test: t => t.trim().split(/\s+/).filter(Boolean).length >= 120,
        good: "Textul conține suficient conținut pentru o verificare inițială.",
        bad: "Textul pare scurt. Verifică dacă ai inclus experiența, educația și competențele."
      }
    ];

    /* TERMENI GENERALI EXCLUȘI DIN COMPARAȚIE */
    const stopWords = new Set(
      "pentru care este sunt acest aceasta acestea unui unei din prin despre către catre după dupa între intre sau și si cu la de în in un o a al ai ale the and with from your you our role job team".split(" ")
    );

    function extractWords(value) {
      return (
        value.toLocaleLowerCase("ro").match(/[a-zăâîșț0-9+#.-]{3,}/giu) || []
      ).filter(word => !stopWords.has(word));
    }

    function escapeHTML(value) {
      return String(value).replace(/[&<>"']/g, character => ({
        "&": "&amp;",
        "<": "&lt;",
        ">": "&gt;",
        '"': "&quot;",
        "'": "&#39;"
      })[character]);
    }

    /* EXTRAGERE TEXT PDF */
    async function extractPDF(file) {
      if (!window.pdfjsLib) {
        throw new Error(
          "Biblioteca PDF nu s-a încărcat. Verifică conexiunea la internet și încearcă din nou."
        );
      }

      const buffer = await file.arrayBuffer();

      const pdf = await pdfjsLib.getDocument({
        data: new Uint8Array(buffer)
      }).promise;

      const pages = [];

      for (let pageNumber = 1; pageNumber <= pdf.numPages; pageNumber++) {
        const page = await pdf.getPage(pageNumber);
        const content = await page.getTextContent();

        pages.push(
          content.items.map(item => item.str).join(" ")
        );
      }

      return pages.join("\n\n").trim();
    }

    /* EXTRAGERE TEXT WORD */
    async function extractDOCX(file) {
      if (!window.mammoth) {
        throw new Error(
          "Biblioteca Word nu s-a încărcat. Verifică conexiunea la internet și încearcă din nou."
        );
      }

      const buffer = await file.arrayBuffer();

      const result = await mammoth.extractRawText({
        arrayBuffer: buffer
      });

      return result.value.trim();
    }

    /* ÎNCĂRCARE DOCUMENT */
    const cvFileInput = $("cvFile");
    const fileStatus = $("fileStatus");
    const cvTextarea = $("cv");

    cvFileInput.addEventListener("change", async function () {
      const file = this.files && this.files[0];

      if (!file) return;

      const extension = file.name.split(".").pop().toLowerCase();

      if (!["pdf", "docx"].includes(extension)) {
        fileStatus.textContent =
          "Format neacceptat. Încarcă un fișier PDF sau DOCX.";
        this.value = "";
        return;
      }

      if (file.size > 10 * 1024 * 1024) {
        fileStatus.textContent =
          "Fișierul este prea mare. Dimensiunea maximă este de 10 MB.";
        this.value = "";
        return;
      }

      fileStatus.textContent = "Documentul se procesează. Te rugăm să aștepți...";

      try {
        let extractedText = "";

        if (extension === "pdf") {
          extractedText = await extractPDF(file);
        } else {
          extractedText = await extractDOCX(file);
        }

        if (!extractedText) {
          throw new Error(
            "Nu am putut extrage text din document. Dacă PDF-ul este scanat ca imagine, este necesară funcția OCR."
          );
        }

        cvTextarea.value = extractedText;

        fileStatus.textContent =
          "Document încărcat cu succes: " + file.name +
          ". Textul CV-ului a fost introdus automat.";

        cvTextarea.scrollIntoView({
          behavior: "smooth",
          block: "center"
        });

      } catch (error) {
        fileStatus.textContent =
          error.message || "A apărut o eroare la citirea documentului.";

        console.error("Eroare încărcare CV:", error);
      }
    });

    /* COMPARAȚIE CU ANUNȚUL */
    function renderKeywords(cvText, jobText) {
      const cvWords = new Set(extractWords(cvText));
      const jobWords = [...new Set(extractWords(jobText))].slice(0, 60);

      const matched = jobWords.filter(word => cvWords.has(word)).slice(0, 25);
      const missing = jobWords.filter(word => !cvWords.has(word)).slice(0, 15);

      let html = `
        <p><strong>${matched.length}</strong> termeni identificați
        și <strong>${missing.length}</strong> termeni care merită verificați manual.</p>
      `;

      if (matched.length) {
        html += `
          <div>
            <strong>Termeni identificați:</strong><br>
            ${matched.map(word => `<span class="tag">${escapeHTML(word)}</span>`).join("")}
          </div>
        `;
      }

      if (missing.length) {
        html += `
          <div style="margin-top:12px">
            <strong>Termeni care nu apar în CV:</strong><br>
            ${missing.map(word => `<span class="tag">${escapeHTML(word)}</span>`).join("")}
          </div>
        `;
      }

      if (!jobWords.length) {
        html += "<p>Nu am identificat suficienți termeni pentru comparație.</p>";
      }

      $("keyword-list").innerHTML = html;
      $("keywords").classList.remove("hidden");
    }

    /* VERIFICARE CV */
    $("check").addEventListener("click", () => {
      const cvText = $("cv").value.trim();
      const jobText = $("job").value.trim();

      if (cvText.length < 40) {
        alert("Te rog să introduci mai mult text din CV pentru o verificare utilă.");
        $("cv").focus();
        return;
      }

      const outcomes = checks.map(item => ({
        ...item,
        ok: item.test(cvText)
      }));

      const score = Math.round(
        outcomes.filter(item => item.ok).length / outcomes.length * 100
      );

      $("score").innerHTML = `${score}<small> / 100</small>`;
      $("bar").style.width = score + "%";

      let description =
        "Folosește recomandările de mai jos pentru a-ți îmbunătăți CV-ul.";

      if (score >= 88) {
        description =
          "Structura verificată include majoritatea elementelor urmărite de instrument.";
      } else if (score >= 63) {
        description =
          "Ai câteva elemente importante prezente. Mai există aspecte de completat.";
      } else {
        description =
          "Sunt mai multe elemente de structură pe care merită să le verifici.";
      }

      $("score-description").textContent = description;

      $("checks").innerHTML = outcomes.map(item => `
        <article class="item">
          <strong>${escapeHTML(item.name)}</strong>
          <span class="status ${item.ok ? "" : "warn"}">
            ${item.ok ? "Identificat" : "De îmbunătățit"}
          </span>
          <p>${escapeHTML(item.ok ? item.good : item.bad)}</p>
        </article>
      `).join("");

      if (jobText) {
        renderKeywords(cvText, jobText);
      } else {
        $("keywords").classList.add("hidden");
      }

      $("results").classList.remove("hidden");

      $("results").scrollIntoView({
        behavior: "smooth",
        block: "start"
      });
    });

    /* ȘTERGERE DATE */
    $("clear").addEventListener("click", () => {
      $("cv").value = "";
      $("job").value = "";
      cvFileInput.value = "";

      fileStatus.textContent = "Nu ai selectat încă un document.";

      $("results").classList.add("hidden");
      $("cv").focus();
    });

    /* DESCHIDERE PDF ÎN MOD COMPATIBIL CU IPHONE */
    function openPDF(blob) {
      const pdfUrl = URL.createObjectURL(blob);

      const isIOS =
        /iPad|iPhone|iPod/.test(navigator.userAgent) ||
        (navigator.platform === "MacIntel" && navigator.maxTouchPoints > 1);

      if (isIOS) {
        // Safari deschide PDF-ul în aceeași filă.
        // Utilizatorul poate folosi apoi Share > Save to Files.
        window.location.href = pdfUrl;
      } else {
        const link = document.createElement("a");
        link.href = pdfUrl;
        link.download = "CARELYNTA-Raport-CV.pdf";
        document.body.appendChild(link);
        link.click();
        link.remove();
      }

      // Nu revocăm imediat adresa PDF: Safari are nevoie de timp să o încarce.
      setTimeout(() => {
        URL.revokeObjectURL(pdfUrl);
      }, 120000);
    }

    /* GENERARE PDF */
    $("print").addEventListener("click", async () => {
      const button = $("print");
      const report = $("results");
      const originalText = button.textContent;

      if (report.classList.contains("hidden")) {
        alert("Te rog să verifici CV-ul înainte de a genera raportul.");
        return;
      }

      if (typeof window.html2pdf !== "function") {
        alert(
          "Biblioteca PDF nu s-a încărcat. Verifică conexiunea la internet și reîncarcă pagina."
        );
        return;
      }

      button.disabled = true;
      button.textContent = "Se pregătește raportul...";

      report.classList.add("pdf-generating");

      try {
        // Lăsăm browserul să aplice stilurile înainte de captură.
        await new Promise(resolve => {
          requestAnimationFrame(() => requestAnimationFrame(resolve));
        });

        const options = {
          margin: [8, 8, 8, 8],
          filename: "CARELYNTA-Raport-CV.pdf",

          image: {
            type: "jpeg",
            quality: 0.95
          },

          html2canvas: {
            scale: 1.5,
            useCORS: true,
            allowTaint: false,
            backgroundColor: "#ffffff",
            logging: false,
            scrollX: 0,
            scrollY: 0
          },

          jsPDF: {
            unit: "mm",
            format: "a4",
            orientation: "portrait",
            compress: true
          },

          pagebreak: {
            mode: ["css", "legacy"],
            avoid: [".item", ".results-header", ".cta"]
          }
        };

        // Capturăm raportul real, vizibil, nu o clonă ascunsă.
        const pdfBlob = await html2pdf()
          .set(options)
          .from(report)
          .outputPdf("blob");

        if (!pdfBlob || pdfBlob.size < 1000) {
          throw new Error("PDF-ul generat nu conține suficiente date.");
        }

        const pdfFile = new File(
          [pdfBlob],
          "CARELYNTA-Raport-CV.pdf",
          { type: "application/pdf" }
        );

        // Pe iPhone și pe browserele compatibile deschidem meniul de partajare.
        let shared = false;

        if (
          navigator.share &&
          navigator.canShare &&
          navigator.canShare({ files: [pdfFile] })
        ) {
          try {
            await navigator.share({
              files: [pdfFile],
              title: "Raport CARELYNTA CV CHECK"
            });

            shared = true;
          } catch (shareError) {
            if (shareError.name === "AbortError") {
              shared = true;
            } else {
              console.warn("Partajarea nu a funcționat:", shareError);
            }
          }
        }

        // Dacă partajarea nu este disponibilă, deschidem PDF-ul.
        if (!shared) {
          openPDF(pdfBlob);
        }

      } catch (error) {
        console.error("Eroare la generarea PDF:", error);

        alert(
          "Nu am putut genera raportul PDF. Verifică conexiunea la internet și încearcă din nou."
        );

      } finally {
        report.classList.remove("pdf-generating");
        button.disabled = false;
        button.textContent = originalText;
      }
    });
  </script>
</body>
</html>
