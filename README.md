<!DOCTYPE html>
<html lang="de">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Realm Germany – Value-Closing-Schulung (Abschluss-Meisterschaft)</title>
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
:root{
  --blue-deep:#0B3D6B;
  --green-dark:#1A6B4A;
  --green-mid:#059669;
  --green-light:#ECFDF5;
  --amber:#F59E0B;
  --red:#DC2626;
  --bg:#F0F2F5;
  --card:#FFFFFF;
  --border:#E5E7EB;
  --text:#1A1A1A;
  --muted:#6B7280;
  --subtle:#F9FAFB;
}
html{scroll-behavior:smooth}
body{font-family:-apple-system,BlinkMacSystemFont,'Segoe UI',Roboto,sans-serif;background:var(--bg);color:var(--text);line-height:1.6}

/* ── HERO ── */
.hero{background:linear-gradient(135deg,#071f38 0%,var(--blue-deep) 45%,var(--green-dark) 100%);color:#fff;padding:4rem 1.5rem 3rem;text-align:center;position:relative;overflow:hidden}
.hero::before{content:'';position:absolute;inset:0;background:url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%23ffffff' fill-opacity='0.03'%3E%3Cpath d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E")}
.hero-badge{display:inline-block;background:rgba(255,255,255,.12);border:1px solid rgba(255,255,255,.2);border-radius:20px;padding:5px 16px;font-size:11px;letter-spacing:2px;text-transform:uppercase;margin-bottom:1.25rem;backdrop-filter:blur(4px)}
.hero h1{font-size:clamp(24px,5vw,42px);font-weight:800;margin-bottom:.75rem;line-height:1.15}
.hero h1 span{color:#6EE7B7}
.hero p{font-size:15px;opacity:.8;max-width:580px;margin:0 auto 2rem}
.hero-stats{display:flex;gap:2rem;justify-content:center;flex-wrap:wrap;margin-top:1.5rem}
.hstat{text-align:center}
.hstat .val{font-size:28px;font-weight:800;color:#6EE7B7}
.hstat .lbl{font-size:11px;opacity:.7;text-transform:uppercase;letter-spacing:1px;margin-top:2px}

/* ── NAV ── */
.nav-wrap{background:#fff;border-bottom:1px solid var(--border);position:sticky;top:0;z-index:100;box-shadow:0 1px 8px rgba(0,0,0,.06)}
.nav-inner{max-width:1100px;margin:0 auto;padding:0 1rem;display:flex;gap:0;overflow-x:auto;scrollbar-width:none}
.nav-inner::-webkit-scrollbar{display:none}
.nav-item{flex-shrink:0;padding:.875rem 1.1rem;font-size:13px;font-weight:600;color:var(--muted);cursor:pointer;border-bottom:3px solid transparent;transition:all .2s;white-space:nowrap}
.nav-item:hover{color:var(--text);background:var(--subtle)}
.nav-item.active{color:var(--green-dark);border-bottom-color:var(--green-dark)}

/* ── LAYOUT ── */
.page{max-width:1100px;margin:0 auto;padding:2rem 1rem}
.section{display:none;animation:fadeIn .3s ease}
.section.active{display:block}
@keyframes fadeIn{from{opacity:0;transform:translateY(8px)}to{opacity:1;transform:translateY(0)}}

/* ── CARDS ── */
.card{background:var(--card);border:1px solid var(--border);border-radius:14px;padding:1.75rem;margin-bottom:1.25rem}
.card-title{font-size:20px;font-weight:800;margin-bottom:1rem;color:var(--blue-deep);display:flex;align-items:center;gap:10px}
.card-title .ico{font-size:24px}
h3{font-size:16px;font-weight:700;margin:1.5rem 0 .6rem;color:var(--text)}
h4{font-size:14px;font-weight:700;margin:.875rem 0 .4rem;color:var(--blue-deep)}
p{font-size:14px;line-height:1.75;color:#374151;margin-bottom:.75rem}
ul,ol{padding-left:1.4rem;margin-bottom:.875rem}
li{font-size:14px;line-height:1.7;color:#374151;margin-bottom:.2rem}
strong{color:var(--text)}

/* ── HIGHLIGHT BOX ── */
.hl{background:var(--green-light);border-left:4px solid var(--green-mid);border-radius:0 10px 10px 0;padding:.875rem 1.1rem;margin:.875rem 0;font-size:13.5px;line-height:1.7}
.hl-amber{background:#FFFBEB;border-left-color:var(--amber)}
.hl-red{background:#FEF2F2;border-left-color:var(--red)}
.hl-blue{background:#EFF6FF;border-left-color:#3B82F6}
.hl strong{display:block;margin-bottom:3px}

/* ── TABLE ── */
.tbl-wrap{overflow-x:auto;margin:.875rem 0;border-radius:10px;border:1px solid var(--border)}
table{width:100%;border-collapse:collapse;font-size:13px}
thead tr{background:var(--subtle)}
th{padding:9px 14px;text-align:left;font-weight:700;color:#374151;border-bottom:1px solid var(--border)}
td{padding:9px 14px;border-bottom:1px solid #F3F4F6;color:#4B5563;vertical-align:top}
tr:last-child td{border-bottom:none}
tr:hover td{background:#FAFAFA}

/* ── STEPS ── */
.steps{margin:.875rem 0}
.step{display:flex;gap:14px;margin-bottom:1rem;align-items:flex-start}
.step-num{width:30px;height:30px;border-radius:50%;background:linear-gradient(135deg,var(--blue-deep),var(--green-dark));color:#fff;font-size:13px;font-weight:800;display:flex;align-items:center;justify-content:center;flex-shrink:0;margin-top:2px}
.step-body h4{font-size:14px;font-weight:700;margin-bottom:3px;color:var(--text)}
.step-body p{font-size:13px;color:var(--muted);margin:0}

/* ── COMPARE TABLE ── */
.vs-grid{display:grid;grid-template-columns:1fr 1fr;gap:12px;margin:1rem 0}
.vs-card{border-radius:12px;padding:1.1rem;border:2px solid transparent}
.vs-realm{background:var(--green-light);border-color:var(--green-mid)}
.vs-comp{background:#F9FAFB;border-color:var(--border)}
.vs-card h4{font-size:14px;font-weight:800;margin-bottom:.75rem}
.vs-card ul{padding-left:1.2rem;margin:0}
.vs-card li{font-size:13px;margin-bottom:3px}

/* ── QUIZ ── */
.quiz-box{background:var(--subtle);border:1px solid var(--border);border-radius:14px;padding:1.5rem;margin-top:1.5rem}
.quiz-box h3{font-size:16px;font-weight:800;margin-bottom:.25rem;color:var(--blue-deep)}
.quiz-box .qsub{font-size:13px;color:var(--muted);margin-bottom:1.25rem}
.qitem{margin-bottom:1.5rem}
.qitem .qt{font-size:14px;font-weight:600;margin-bottom:.6rem;line-height:1.5}
.qopt{display:flex;align-items:flex-start;gap:9px;background:#fff;border:1.5px solid var(--border);border-radius:9px;padding:.6rem .875rem;cursor:pointer;margin-bottom:6px;font-size:13px;color:#374151;width:100%;text-align:left;line-height:1.5;transition:all .15s}
.qopt:hover{border-color:#9CA3AF;background:var(--subtle)}
.qopt .qdot{width:15px;height:15px;border:2px solid #D1D5DB;border-radius:50%;flex-shrink:0;margin-top:2px;transition:all .15s}
.qopt.correct{background:var(--green-light);border-color:var(--green-mid);color:#065F46}
.qopt.correct .qdot{background:var(--green-mid);border-color:var(--green-mid)}
.qopt.wrong{background:#FEF2F2;border-color:var(--red);color:#7F1D1D}
.qopt.wrong .qdot{background:var(--red);border-color:var(--red)}
.qopt.locked{pointer-events:none}
.qfb{display:none;font-size:12px;line-height:1.6;padding:.55rem .875rem;border-radius:8px;margin-top:.4rem}
.qfb.show{display:block}
.qfb.ok{background:var(--green-light);color:#065F46;border:1px solid #A7F3D0}
.qfb.err{background:#FEF2F2;color:#7F1D1D;border:1px solid #FECACA}
.quiz-score{display:none;background:#fff;border-radius:10px;padding:1.5rem;text-align:center;margin-top:1rem;border:1px solid var(--border)}
.quiz-score.show{display:block}
.quiz-score .qs-val{font-size:40px;font-weight:800;color:var(--green-dark)}
.quiz-score .qs-lbl{font-size:13px;color:var(--muted)}
.name-row{display:flex;align-items:center;gap:12px;background:#fff;border:1.5px solid var(--border);border-radius:10px;padding:.75rem 1rem;margin-bottom:1.5rem}
.name-row label{font-size:14px;font-weight:700;white-space:nowrap;color:var(--green-dark)}
.name-row input{flex:1;border:none;background:transparent;font-size:14px;color:var(--text);outline:none}
.name-row input::placeholder{color:var(--muted)}

/* ── PROGRESS NAV BTN ── */
.nav-btns{display:flex;justify-content:space-between;margin-top:2rem;gap:10px}
.btn{padding:.65rem 1.4rem;border-radius:10px;border:1.5px solid var(--border);background:#fff;cursor:pointer;font-size:14px;font-weight:700;color:var(--text);transition:all .2s;display:inline-flex;align-items:center;gap:6px}
.btn:hover{background:var(--subtle);border-color:#9CA3AF}
.btn-primary{background:linear-gradient(135deg,var(--blue-deep),var(--green-dark));color:#fff;border-color:transparent}
.btn-primary:hover{opacity:.9;background:linear-gradient(135deg,var(--blue-deep),var(--green-dark))}

/* ── PROGRESS BAR ── */
.sect-progress{background:var(--border);border-radius:8px;height:5px;margin-bottom:2rem}
.sect-progress-fill{background:linear-gradient(90deg,var(--blue-deep),var(--green-dark));border-radius:8px;height:5px;transition:width .5s}

@media(max-width:600px){
  .vs-grid{grid-template-columns:1fr}
  .hero-stats{gap:1.25rem}
}
</style>
</head>
<body>

<!-- HERO -->
<div class="hero">
  <div class="hero-badge">Realm Germany · Phase 3 Masterclass</div>
  <h1>Phase 3: Die <span>Value-Closing-Schulung</span></h1>
  <p>Die psychologische Abschluss-Meisterschaft im Investitionsgüter- und High-Ticket B2B-Vertrieb. Vom strategischen Einwand-Slam bis zur finalen Sign-on-Architektur.</p>
  <div class="hero-stats">
    <div class="hstat"><div class="val">3</div><div class="lbl">Kernbereiche</div></div>
    <div class="hstat"><div class="val">100%</div><div class="lbl">Abschluss-Fokus</div></div>
    <div class="hstat"><div class="val">0%</div><div class="lbl">Druck-Verkauf</div></div>
    <div class="hstat"><div class="val">ROI</div><div class="lbl">Wert-Argumentation</div></div>
  </div>
</div>

<!-- NAV -->
<div class="nav-wrap">
  <div class="nav-inner">
    <div class="nav-item active" onclick="goSec(0)">1 · Psychologische Einwandbehandlung</div>
    <div class="nav-item" onclick="goSec(1)">2 · Realm Value-Pricing</div>
    <div class="nav-item" onclick="goSec(2)">3 · Abschluss-Trigger &amp; Closing</div>
    <div class="nav-item" onclick="goSec(3)">4 · Abschluss-Prüfung</div>
  </div>
</div>

<div class="page">

<!-- ══════════════════════════════ SECTION 0 ══ -->
<div class="section active" id="sec0">
  <div class="sect-progress"><div class="sect-progress-fill" style="width:33%"></div></div>

  <div class="card">
    <div class="card-title"><span class="ico">⚔️</span>Modul 1: Advanced Einwandbehandlung &amp; Vorwands-Isolation</div>
    <p>Im High-Ticket B2B-Vertrieb sind Einwände oft nur vorgeschobene Schutzschilde (Vorwände). Dieses Modul liefert die psychologischen Hebel, um diese Schilde im laufenden Gespräch zu isolieren, umzudrehen und als Hebel für den Abschluss zu nutzen.</p>

    <div class="hl"><strong>Das eiserne Gesetz der Isolation:</strong> Behandle niemals einen Einwand, bevor du nicht sichergestellt hast, dass es der <em>echte</em> und <em>einzige</em> Grund ist, der dem Abschluss im Weg steht. Wer zu früh argumentiert, jagt Geister.</div>

    <h3>Die 3 klassischen High-Ticket-Einwände &amp; die Drehkreuz-Konter</h3>

    <div class="hl-amber">
      <strong>Vorwand 1: „Wir haben aktuell absolut keine Zeit dafür / Unsere Kapazitäten sind voll."</strong>
      <p><em>Die psychologische Isolation:</em> „Ich verstehe vollkommen, dass Ihre Auftragsbücher voll sind. Angenommen, Zeit spielte keine Rolle, weil unser System sich praktisch von alleine implementiert und ab Woche 1 messbar Zeit einspart – gäbe es dann noch einen anderen Grund, warum wir das Projekt jetzt nicht anpacken sollten?“</p>
      <p><strong>Der Hebel-Konter:</strong> „Genau <em>weil</em> Sie keine Zeit haben, müssen wir jetzt handeln. Wenn Sie weiterhin auf die herkömmlichen, manuellen Prozesse setzen, fressen Ihnen die alten Strukturen jeden Tag wertvolle Stunden weg. Realm automatisiert genau diese zeitraubenden Schritte. Sie investieren jetzt einmalig 3 Stunden Aufwand, um ab nächsten Monat dauerhaft 15 Stunden pro Woche einzusparen. Wann, wenn nicht bei voller Auslastung, ist der richtige Zeitpunkt, Ineffizienz zu eliminieren?“</p>
    </div>

    <div class="hl-amber">
      <strong>Vorwand 2: „Das System ist uns zu teuer / Dafür haben wir aktuell kein Budget."</strong>
      <p><em>Die psychologische Isolation:</em> „Wenn wir den Preis für einen kurzen Moment ausblenden und das System würde sich nachweislich durch die Ersparnisse selbst finanzieren – ist Realm dann die Lösung, die Sie für Ihren Betrieb strategisch haben wollen?“</p>
      <p><strong>Der Hebel-Konter:</strong> „Ein System wie Realm ist kein Kostenfaktor, sondern eine Investition. Wenn Sie mir sagen, es ist zu teuer, bedeutet das meistens: Der messbare Ertrag ist im Vergleich zum Preis noch nicht greifbar genug. Lassen Sie uns die Zahlen aufmachen: Wenn wir durch die Implementierung Ihre Betriebskosten um monatlich 4.500 € senken, die Investition aber auf 2.000 € monatlich skaliert ist – ist das System dann immer noch teuer, oder verdient es ab dem ersten Tag Geld für Sie?“</p>
    </div>

    <div class="hl-amber">
      <strong>Vorwand 3: „Wir sind bereits seit Jahren mit einem Partner aufgestellt und voll zufrieden."</strong>
      <p><em>Die psychologische Isolation:</em> „Es spricht absolut für Sie, dass Sie auf langfristige Partnerschaften setzen. Wenn wir eine Zusammenarbeit starten, erwarte ich gar nicht, dass Sie Ihren bestehenden Partner sofort ersetzen. Wenn wir Ihnen aber in einem spezifischen Teilbereich einen unfairen Marktvorteil bieten können – wären Sie grundsätzlich offen für ein strategisches Zweitstandbein?“</p>
      <p><strong>Der Hebel-Konter:</strong> „Genau diese Zufriedenheit wollen wir sichern. Die erfolgreichsten Unternehmen im Markt verlassen sich jedoch nie nur auf eine einzige Pipeline. Eine strategische Redundanz schützt Sie vor Lieferengpässen, Preisdiktaten oder technologischem Stillstand. Realm setzt da an, wo Ihr aktueller Partner an seine Grenzen stößt – ohne dass Sie Bewährtes direkt über Bord werfen müssen. Lassen Sie uns mit einem risikofreien Testprojekt starten.“</p>
    </div>
  </div>

  <div class="nav-btns">
    <div></div>
    <button class="btn btn-primary" onclick="goSec(1)">Weiter: Realm Value-Pricing →</button>
  </div>
</div>

<!-- ══════════════════════════════ SECTION 1 ══ -->
<div class="section" id="sec1">
  <div class="sect-progress"><div class="sect-progress-fill" style="width:66%"></div></div>

  <div class="card">
    <div class="card-title"><span class="ico">💎</span>Modul 2: Die Realm Value-Pricing-Strategie (ROI-Präsentation)</div>
    <p>Wer High-Ticket-Investitionsgüter über den Preis verkauft, verliert gegen Billiganbieter. Bei der Value-Pricing-Strategie verschieben wir den Fokus radikal: weg vom Preisschild, hin zu den Kosten des Nicht-Handelns (Cost of Inaction).</p>
    
    <div class="vs-grid">
      <div class="vs-card vs-comp">
        <h4>Die falsche Methode: Feature-Katalog</h4>
        <ul>
          <li>Nennung des Gesamtpreises am Ende des Termins.</li>
          <li>Erklärung aller technischen Komponenten und Details.</li>
          <li>Rechtfertigung des Preises durch Materialqualität.</li>
          <li>Resultat: Der Kunde vergleicht die nackten Kosten mit Mitbewerbern.</li>
        </ul>
      </div>
      <div class="vs-card vs-realm">
        <h4>Die Realm-Methode: Wert-Rahmung</h4>
        <ul>
          <li>Vollständige Transparenz über den finanziellen Hebel.</li>
          <li>Fokus auf die vermiedenen Verluste und Umsatzsteigerungen.</li>
          <li>Präsentation des Preises als reine Bruchteils-Investition des ROI.</li>
          <li>Resultat: Die Kosten des Abwartens sind höher als die Investition.</li>
        </ul>
      </div>
    </div>

    <h3>Die ROI-Formel in der Gesprächspraxis</h3>
    <p>Um den Premium-Preis im Kopf des Kunden komplett in den Schatten zu stellen, nutzen wir das Prinzip der **monetären Kontrastierung**:</p>

    <div class="hl-blue">
      <strong>Die mathematische Zwinge:</strong>
      <p>„Herr [Name], das Gesamtsystem erfordert eine einmalige Investition von 45.000 €. Auf den ersten Blick eine stattliche Summe. Lassen Sie uns das dem gegenüberstellen, was aktuell jeden Monat laut Ihren Angaben ungenutzt verpufft:</p>
      <ul>
        <li>Durch unoptimierte Prozesse verlieren Sie monatlich knapp 2.500 € an Arbeitszeit.</li>
        <li>Durch mangelnde Performance gehen Ihnen schätzungsweise 2 Projekte pro Quartal verloren – das sind umgerechnet 4.000 € entgangener Rohertrag pro Monat.</li>
      </ul>
      <p>Das bedeutet: **Sie zahlen aktuell bereits 6.500 € jeden Monat dafür, dass Sie Realm NICHT nutzen.** In weniger als 7 Monaten hat sich das System vollständig amortisiert. Ab diesem Zeitpunkt fließt diese Summe eins zu eins als Reingewinn in Ihren Betrieb. Ist es betriebswirtschaftlich sinnvoll, diese 6.500 € nächsten Monat wieder zu verbrennen?“</p>
    </div>
  </div>

  <div class="nav-btns">
    <button class="btn" onclick="goSec(0)">← Zurück</button>
    <button class="btn btn-primary" onclick="goSec(2)">Weiter: Abschluss-Trigger →</button>
  </div>
</div>

<!-- ══════════════════════════════ SECTION 2 ══ -->
<div class="section" id="sec2">
  <div class="sect-progress"><div class="sect-progress-fill" style="width:100%"></div></div>

  <div class="card">
    <div class="card-title"><span class="ico">🤝</span>Modul 3: Abschluss-Trigger &amp; Partnerschaftliche Closing-Techniken</div>
    <p>Ein echter Spitzenverkäufer drückt den Kunden nicht in eine Entscheidung, sondern führt ihn logisch und elegant dorthin. Wenn die Argumentation der vorherigen Module steht, ist das Closing nur noch die formale Bestätigung einer bereits getroffenen inneren Entscheidung.</p>

    <h3>Die 3 stärksten Closing-Schleifen</h3>

    <div class="steps">
      <div class="step">
        <div class="step-num">1</div>
        <div class="step-body">
          <h4>Die logische Konsequenz-Frage (The Logical Next Step)</h4>
          <p>Diese Technik baut auf den zuvor bestätigten Mehrwerten auf und führt direkt in die logische Umsetzung.</p>
          <p><em>Skript-Vorlage:</em> „Herr [Name], wir haben gesehen, dass das System Ihre Kapazitätsengpässe löst und sich betriebswirtschaftlich in knapp 7 Monaten von selbst trägt. Menschlich passt es auf beiden Seiten ebenfalls hervorragend. Was spricht aus Ihrer Sicht vernünftigerweise dagegen, dass wir das Projekt jetzt genau so in die Wege leiten?“</p>
        </div>
      </div>
      <div class="step">
        <div class="step-num">2</div>
        <div class="step-body">
          <h4>Der „Risk-Reversal“-Abschluss (Die vollständige Sicherheitsgarantie)</h4>
          <p>Perfekt geeignet für Kunden, die zwar überzeugt sind, aber kurz vor der Unterschrift eine letzte rationale Blockade aufbauen.</p>
          <p><em>Skript-Vorlage:</em> „Ich merke, Sie wollen absolut sichergehen, dass die Implementierung reibungslos läuft. Lassen Sie uns das Risiko komplett vom Tisch nehmen: Wir halten im Vertrag explizit fest, dass wir innerhalb der ersten 30 Tage ein Sonderkündigungsrecht einräumen, falls die vereinbarten Meilensteine unsererseits nicht eingehalten werden. Wenn wir das Risiko somit vollständig auf unsere Schultern nehmen – steht einem gemeinsamen Start dann noch etwas im Wege?“</p>
        </div>
      </div>
      <div class="step">
        <div class="step-num">3</div>
        <div class="step-body">
          <h4>Die bilaterale Implementierungs-Weiche (Die Detail-Lenkung)</h4>
          <p>Man stellt nicht mehr die Frage, *ob* der Kunde kauft, sondern *wie* die Zusammenarbeit gestartet wird. Das impliziert den Abschluss psychologisch.</p>
          <p><em>Skript-Vorlage:</em> „Herr [Name], um den Übergang für Ihr Team so reibungslos wie möglich zu gestalten, haben wir zwei Optionen: Wollen wir planmäßig direkt in der kommenden Woche mit dem technischen Kick-off starten, oder macht es für Sie mehr Sinn, wenn wir die Datenmigration im Hintergrund vorbereiten und offiziell zum Ersten des Folgemonats live gehen?“</p>
        </div>
      </div>
    </div>
  </div>

  <div class="nav-btns">
    <button class="btn" onclick="goSec(1)">← Zurück</button>
    <button class="btn btn-primary" onclick="goSec(3)">Weiter: Abschluss-Prüfung →</button>
  </div>
</div>

<!-- ══════════════════════════════ SECTION 3 ══ -->
<div class="section" id="sec3">
  <div class="sect-progress"><div class="sect-progress-fill" style="width:100%"></div></div>

  <div class="card">
    <div class="card-title"><span class="ico">🏆</span>Abschluss-Prüfung: Kannst du den Sack zumachen?</div>
    <p>4 praxisnahe B2B-High-Ticket-Szenarien aus der Value-Closing-Phase. Nur lösbar, wenn du die psychologischen Mechanismen fehlerfrei anwenden kannst.</p>
  </div>

  <div class="quiz-box">
    <h3>⚔️ Value-Closing-Zertifizierung – Abschlussprüfung</h3>
    <div class="qsub">4 Szenarien · Professionelles B2B-Niveau · Bestehen ab 3/4 korrekten Antworten</div>

    <div class="name-row">
      <label for="qename">👤 Dein Name:</label>
      <input type="text" id="qename" placeholder="Vor- und Nachname eingeben …" autocomplete="name" />
    </div>

    <div class="qitem" id="qq1">
      <div class="qt">1. Ein potenzieller B2B-Kunde sagt abrupt: „Das klingt alles gut, aber schicken Sie mir einfach mal die Unterlagen per Mail zu, ich schaue mir das nächste Woche an." Wie reagiert ein geschulter Realm-Closer?</div>
      <button class="qopt" onclick="qpick(this,1,'a')"><span class="qdot"></span>Ich willige sofort ein, sende die Mail und vereinbare direkt einen Nachfass-Termin für die darauffolgende Woche.</button>
      <button class="qopt" onclick="qpick(this,1,'b')"><span class="qdot"></span>Ich isoliere den Vorwand direkt: „Gerne sende ich Ihnen die Unterlagen. Wenn wir die Dokumente kurz beiseitelegen: Gibt es abgesehen vom Durchschauen der Unterlagen noch etwas, das einem gemeinsamen Start im Weg steht?"</button>
      <button class="qopt" onclick="qpick(this,1,'c')"><span class="qdot"></span>Ich sage ihm direkt, dass das Zusenden von Unterlagen meistens nichts bringt und wir jetzt eine Entscheidung brauchen.</button>
      <div class="qfb ok" id="qfb1ok">✓ Exzellent! Du hast den Vorwand isoliert. Das unkommentierte Versenden von Unterlagen führt fast immer zu einer toten Pipeline. Indem du fragst, was *abgesehen davon* im Weg steht, findest du heraus, ob echter Informationsbedarf besteht oder ob es sich um ein höfliches Abwimmeln handelt.</div>
      <div class="qfb err" id="qfb1err">✗ Falscher Ansatz. Option A führt direkt in die unverbindliche Geister-Pipeline. Option C wirkt aggressiv und unprofessionell. Die korrekte Antwort ist B, um den wahren Kern des Zögerns freizulegen.</div>
    </div>

    <div class="qitem" id="qq2">
      <div class="qt">2. Was ist das Kernprinzip der Realm "Value-Pricing-Strategie" bei der Präsentation von hohen Investitionskosten?</div>
      <button class="qopt" onclick="qpick(this,2,'a')"><span class="qdot"></span>Man rabattiert den Preis sofort um 10 %, um dem Kunden ein schnelles Erfolgserlebnis zu vermitteln.</button>
      <button class="qopt" onclick="qpick(this,2,'b')"><span class="qdot"></span>Man bricht die Kosten auf einen extrem kleinen Tagespreis herunter (z. B. "nur ein Kaffee am Tag"), um den Preis unbedeutend wirken zu lassen.</button>
      <button class="qopt" onclick="qpick(this,2,'c')"><span class="qdot"></span>Man stellt den Investitionskosten die "Cost of Inaction" (Kosten des Nicht-Handelns) gegenüber, sodass das Abwarten für das Unternehmen teurer ist als die Investition selbst.</button>
      <div class="qfb ok" id="qfb2ok">✓ Perfekt! B2B-Entscheider reagieren auf betriebswirtschaftliche Logik. Wenn du glasklar aufzeigst, dass das Verbleiben im Ist-Zustand pro Monat mehr Geld verbrennt als die Amortisationsrate des neuen Systems, wird die Investition zur logisch zwingenden Entscheidung.</div>
      <div class="qfb err" id="qfb2err">✗ Falsch. Rabatte (A) zerstören den Premium-Status und deine Marge. Die Kaffee-Metapher (B) funktioniert im B2C-Bereich, wirkt aber im gehobenen B2B-Vertrieb oft unprofessionell. Die richtige Antwort ist C.</div>
    </div>

    <div class="qitem" id="qq3">
      <div class="qt">3. Der Kunde sagt: „Ihr System ist toll, aber wir arbeiten seit 10 Jahren mit unserem aktuellen Partner zusammen. Ein Wechsel kommt nicht infrage." Welchen Hebel nutzt du?</div>
      <button class="qopt" onclick="qpick(this,3,'a')"><span class="qdot"></span>Ich rede den aktuellen Partner schlecht und liste die technologischen Defizite der Konkurrenz auf.</button>
      <button class="qopt" onclick="qpick(this,3,'b')"><span class="qdot"></span>Ich akzeptiere die Absage respektvoll und bitte darum, in zwei Jahren noch einmal anrufen zu dürfen.</button>
      <button class="qopt" onclick="qpick(this,3,'c')"><span class="qdot"></span>Ich lobe seine Treue und positioniere Realm strategisch als risikoarmes, innovatives Zweitstandbein zur Absicherung und Redundanz, ohne den Erstpartner direkt zu kündigen.</button>
      <div class="qfb ok" id="qfb3ok">✓ Ganz genau! Das Aufbrechen von langjährigen Partnerschaften gelingt selten per Frontalangriff. Die Positionierung als komplementäres Zweitstandbein senkt die psychologische Wechselbarriere gegen Null und öffnet dir die Tür für das erste Testprojekt.</div>
      <div class="qfb err" id="qfb3err">✗ Nicht optimal. Das Schlechtreden des Mitbewerbers (A) erzeugt sofort Reaktanz beim Kunden, da es seine bisherigen Entscheidungen angreift. Kampflos aufzugeben (B) ist kein Closing. Antwort C ist der strategische Königsweg.</div>
    </div>

    <div class="qitem" id="qq4">
      <div class="qt">4. Du hast alle Einwände gelöst, die Präsentation war ein voller Erfolg, doch der Kunde zögert am finalen Punkt. Welche Closing-Schleife ist jetzt angebracht, um partnerschaftlich den Sack zuzumachen?</div>
      <button class="qopt" onclick="qpick(this,4,'a')"><span class="qdot"></span>„Möchten Sie den Vertrag jetzt unterschreiben oder brauchen Sie noch Bedenkzeit?"</button>
      <button class="qopt" onclick="qpick(this,4,'b')"><span class="qdot"></span>„Was spricht aus Ihrer Sicht vernünftigerweise dagegen, dass wir das Projekt jetzt genau so in die Wege leiten?" (Die logische Konsequenz-Frage)</button>
      <button class="qopt" onclick="qpick(this,4,'c')"><span class="qdot"></span>„Wenn Sie heute nicht unterschreiben, kann ich Ihnen diesen Aktionspreis leider nicht mehr garantieren."</button>
      <div class="qfb ok" id="qfb4ok">✓ Großartig! Die logische Konsequenz-Frage fordert den Kunden heraus, einen *vernünftigen* Grund für ein Nein zu nennen. Da alle Einwände zuvor isoliert und gelöst wurden, gibt es rational kein Argument mehr – der Weg für die Unterschrift ist frei.</div>
      <div class="qfb err" id="qfb3err">✗ Knappe Fehlentscheidung. Option A bietet dem Kunden eine künstliche Ausstiegsrampe ("Bedenkzeit"). Option C ist künstlicher Druck ("Drückermethode"), der im High-Ticket B2B-Segment das Vertrauen nachhaltig beschädigt. Die richtige Wahl ist B.</div>
    </div>

    <div class="quiz-score" id="qscorebox">
      <div class="qs-val" id="qscoreval">0 / 4</div>
      <div class="qs-lbl" id="qscorelbl">Ergebnis</div>
      <div id="qscoretext" style="margin-top:10px; font-weight:700; font-size:14px"></div>
    </div>
  </div>

  <div class="nav-btns">
    <button class="btn" onclick="goSec(2)">← Zurück</button>
    <div></div>
  </div>
</div>

</div>

<script>
// NAVIGATION SYSTEM
const sections = document.querySelectorAll('.section');
const navItems = document.querySelectorAll('.nav-item');

function goSec(idx) {
  sections.forEach((s, i) => {
    if(i === idx) {
      s.classList.add('active');
      navItems[i].classList.add('active');
      navItems[i].scrollIntoView({ behavior: 'smooth', block: 'nearest', inline: 'center' });
    } else {
      s.classList.remove('active');
      navItems[i].classList.remove('active');
    }
  });
  window.scrollTo({ top: 0, behavior: 'smooth' });
}

// QUIZ ENGINE
const userAnswers = {};
const correctAnswers = { 1: 'b', 2: 'c', 3: 'c', 4: 'b' };

function qpick(btn, qNum, option) {
  const parent = document.getElementById('qq' + qNum);
  const options = parent.querySelectorAll('.qopt');
  
  options.forEach(opt => opt.classList.add('locked'));
  
  userAnswers[qNum] = option;
  
  const isCorrect = option === correctAnswers[qNum];
  if(isCorrect) {
    btn.classList.add('correct');
    document.getElementById('qfb' + qNum + 'ok').classList.add('show');
  } else {
    btn.classList.add('wrong');
    document.getElementById('qfb' + qNum + 'err').classList.add('show');
    options.forEach(opt => {
      if(opt.getAttribute('onclick').includes(`'${correctAnswers[qNum]}'`)) {
        opt.classList.add('correct');
      }
    });
  }
  
  checkQuizScore();
}

function checkQuizScore() {
  const answeredCount = Object.keys(userAnswers).length;
  if(answeredCount === 4) {
    let score = 0;
    for(let q in correctAnswers) {
      if(userAnswers[q] === correctAnswers[q]) score++;
    }
    
    const scoreBox = document.getElementById('qscorebox');
    const scoreVal = document.getElementById('qscoreval');
    const scoreText = document.getElementById('qscoretext');
    const name = document.getElementById('qename').value.trim() || 'Zukünftiger Master-Closer';
    
    scoreVal.innerText = score + " / 4";
    scoreBox.classList.add('show');
    
    if(score >= 3) {
      scoreText.innerHTML = `🎉 Erstklassig, ${name}! Du hast die Value-Closing Prüfung BESTANDEN! Du besitzt die Werkzeuge, um Abschlüsse auf Top-Niveau souverän zu versiegeln.`;
      scoreText.style.color = "var(--green-dark)";
    } else {
      scoreText.innerHTML = `⚠️ Kopf hoch, ${name}. Du hast die Bestehensgrenze knapp verfehlt. Analysiere noch einmal die ROI-Logiken und versuche es erneut!`;
      scoreText.style.color = "var(--red)";
    }
  }
}
</script>
</body>
</html>
