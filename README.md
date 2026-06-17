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
.hero p{font-size:15px;opacity:.8;max-width:640px;margin:0 auto 2rem}
.hero-stats{display:flex;gap:2rem;justify-content:center;flex-wrap:wrap;margin-top:1.5rem}
.hstat{text-align:center}
.hstat .val{font-size:28px;font-weight:800;color:#6EE7B7}
.hstat .lbl{font-size:11px;opacity:.7;text-transform:uppercase;letter-spacing:1px;margin-top:2px}

/* ── NAV ── */
.nav-wrap{background:#fff;border-bottom:1px solid var(--border);position:sticky;top:0;z-index:100;box-shadow:0 1px 8px rgba(0,0,0,.06)}
.nav-inner{max-width:1200px;margin:0 auto;padding:0 1rem;display:flex;gap:0;overflow-x:auto;scrollbar-width:none}
.nav-inner::-webkit-scrollbar{display:none}
.nav-item{flex-shrink:0;padding:.875rem 1.1rem;font-size:13px;font-weight:600;color:var(--muted);cursor:pointer;border-bottom:3px solid transparent;transition:all .2s;white-space:nowrap}
.nav-item:hover{color:var(--text);background:var(--subtle)}
.nav-item.active{color:var(--green-dark);border-bottom-color:var(--green-dark)}

/* ── LAYOUT ── */
.page{max-width:1200px;margin:0 auto;padding:2rem 1rem}
.section{display:none;animation:fadeIn .3s ease}
.section.active{display:block}
@keyframes fadeIn{from{opacity:0;transform:translateY(8px)}to{opacity:1;transform:translateY(0)}}

/* ── CARDS ── */
.card{background:var(--card);border:1px solid var(--border);border-radius:14px;padding:2rem;margin-bottom:1.5rem}
.card-title{font-size:22px;font-weight:800;margin-bottom:1.25rem;color:var(--blue-deep);display:flex;align-items:center;gap:10px;border-bottom:1px solid var(--border);padding-bottom:0.75rem}
.card-title .ico{font-size:26px}
h3{font-size:18px;font-weight:700;margin:1.75rem 0 .75rem;color:var(--blue-deep);display:flex;align-items:center;gap:6px}
h4{font-size:15px;font-weight:700;margin:1.25rem 0 .5rem;color:var(--text)}
p{font-size:14.5px;line-height:1.8;color:#374151;margin-bottom:1rem}
ul,ol{padding-left:1.5rem;margin-bottom:1rem}
li{font-size:14.5px;line-height:1.75;color:#374151;margin-bottom:.3rem}
strong{color:var(--text)}

/* ── HIGHLIGHT BOX ── */
.hl{background:var(--green-light);border-left:4px solid var(--green-mid);border-radius:0 10px 10px 0;padding:1.1rem;margin:1.25rem 0;font-size:14px;line-height:1.75}
.hl-amber{background:#FFFBEB;border-left-color:var(--amber)}
.hl-red{background:#FEF2F2;border-left-color:var(--red)}
.hl-blue{background:#EFF6FF;border-left-color:#3B82F6}
.hl strong{display:block;margin-bottom:5px;font-size:15px;color:var(--text)}

/* ── CODE / SCRIPT BOX ── */
.script-box{background:#F8FAFC;border:1px dashed #CBD5E1;border-radius:8px;padding:1.25rem;margin:1rem 0;font-family:inherit}
.script-tag{display:inline-block;background:#E2E8F0;color:#475569;font-size:11px;font-weight:700;padding:2px 8px;border-radius:4px;text-transform:uppercase;margin-bottom:0.5rem}

/* ── COMPARE TABLE ── */
.vs-grid{display:grid;grid-template-columns:1fr 1fr;gap:16px;margin:1.25rem 0}
.vs-card{border-radius:12px;padding:1.25rem;border:2px solid transparent}
.vs-realm{background:var(--green-light);border-color:var(--green-mid)}
.vs-comp{background:#F9FAFB;border-color:var(--border)}
.vs-card h4{font-size:15px;font-weight:800;margin-bottom:.75rem;color:var(--blue-deep)}
.vs-card ul{padding-left:1.2rem;margin:0}
.vs-card li{font-size:13.5px;margin-bottom:4px}

/* ── QUIZ ── */
.quiz-box{background:var(--subtle);border:1px solid var(--border);border-radius:14px;padding:2rem;margin-top:2rem}
.quiz-box h3{font-size:18px;font-weight:800;margin-bottom:.25rem;color:var(--blue-deep)}
.quiz-box .qsub{font-size:14px;color:var(--muted);margin-bottom:1.5rem}
.qitem{margin-bottom:2rem}
.qitem .qt{font-size:15px;font-weight:600;margin-bottom:.75rem;line-height:1.6}
.qopt{display:flex;align-items:flex-start;gap:11px;background:#fff;border:1.5px solid var(--border);border-radius:9px;padding:.75rem 1rem;cursor:pointer;margin-bottom:8px;font-size:14px;color:#374151;width:100%;text-align:left;line-height:1.5;transition:all .15s}
.qopt:hover{border-color:#9CA3AF;background:var(--subtle)}
.qopt .qdot{width:16px;height:16px;border:2px solid #D1D5DB;border-radius:50%;flex-shrink:0;margin-top:2px;transition:all .15s}
.qopt.correct{background:var(--green-light);border-color:var(--green-mid);color:#065F46}
.qopt.correct .qdot{background:var(--green-mid);border-color:var(--green-mid)}
.qopt.wrong{background:#FEF2F2;border-color:var(--red);color:#7F1D1D}
.qopt.wrong .qdot{background:var(--red);border-color:var(--red)}
.qopt.locked{pointer-events:none}
.qfb{display:none;font-size:13px;line-height:1.6;padding:.75rem 1.1rem;border-radius:8px;margin-top:.5rem}
.qfb.show{display:block}
.qfb.ok{background:var(--green-light);color:#065F46;border:1px solid #A7F3D0}
.qfb.err{background:#FEF2F2;color:#7F1D1D;border:1px solid #FECACA}
.quiz-score{display:none;background:#fff;border-radius:10px;padding:2rem;text-align:center;margin-top:1.5rem;border:1px solid var(--border)}
.quiz-score.show{display:block}
.quiz-score .qs-val{font-size:44px;font-weight:800;color:var(--green-dark)}
.quiz-score .qs-lbl{font-size:14px;color:var(--muted)}
.name-row{display:flex;align-items:center;gap:12px;background:#fff;border:1.5px solid var(--border);border-radius:10px;padding:.75rem 1rem;margin-bottom:2rem}
.name-row label{font-size:14px;font-weight:700;white-space:nowrap;color:var(--green-dark)}
.name-row input{flex:1;border:none;background:transparent;font-size:14px;color:var(--text);outline:none}
.name-row input::placeholder{color:var(--muted)}

/* ── PROGRESS & BUTTONS ── */
.nav-btns{display:flex;justify-content:space-between;margin-top:2.5rem;gap:12px}
.btn{padding:.75rem 1.5rem;border-radius:10px;border:1.5px solid var(--border);background:#fff;cursor:pointer;font-size:14px;font-weight:700;color:var(--text);transition:all .2s;display:inline-flex;align-items:center;gap:8px}
.btn:hover{background:var(--subtle);border-color:#9CA3AF}
.btn-primary{background:linear-gradient(135deg,var(--blue-deep),var(--green-dark));color:#fff;border-color:transparent}
.btn-primary:hover{opacity:.9}
.sect-progress{background:var(--border);border-radius:8px;height:6px;margin-bottom:2.5rem}
.sect-progress-fill{background:linear-gradient(90deg,var(--blue-deep),var(--green-dark));border-radius:8px;height:6px;transition:width .5s}

@media(max-width:768px){
  .vs-grid{grid-template-columns:1fr}
  .hero-stats{gap:1.5rem}
}
</style>
</head>
<body>

<!-- HERO -->
<div class="hero">
  <div class="hero-badge">Realm Germany · Phase 3 Masterclass</div>
  <h1>Phase 3: Die <span>Value-Closing-Schulung</span></h1>
  <p>Das vollständige 7-Module-System zur psychologischen Abschluss-Meisterschaft im Investitionsgüter- und High-Ticket B2B-Vertrieb. Konzipiert für eine Bearbeitungszeit von ca. 45 Minuten.</p>
  <div class="hero-stats">
    <div class="hstat"><div class="val">7</div><div class="lbl">Spezial-Module</div></div>
    <div class="hstat"><div class="val">45 min</div><div class="lbl">Intensiv-Fokus</div></div>
    <div class="hstat"><div class="val">B2B</div><div class="lbl">Enterprise ROI</div></div>
    <div class="hstat"><div class="val">100%</div><div class="lbl">Praxis-Skripte</div></div>
  </div>
</div>

<!-- NAV -->
<div class="nav-wrap">
  <div class="nav-inner">
    <div class="nav-item active" onclick="goSec(0)">M1-M2: Einwand-Isolation</div>
    <div class="nav-item" onclick="goSec(1)">M3-M4: Value-Pricing &amp; ROI</div>
    <div class="nav-item" onclick="goSec(2)">M5-M6: Closing &amp; Einwände</div>
    <div class="nav-item" onclick="goSec(3)">M7: Finaler Vertrag &amp; Prüfung</div>
  </div>
</div>

<div class="page">

<!-- ══════════════════════════════ SECTION 0 (M1-M2) ══ -->
<div class="section active" id="sec0">
  <div class="sect-progress"><div class="sect-progress-fill" style="width:25%"></div></div>

  <!-- MODUL 1 -->
  <div class="card">
    <div class="card-title"><span class="ico">🔍</span>Modul 1: Die Psychologie des B2B-Zögerns &amp; Vorwands-Erkennung</div>
    <p>Im gehobenen B2B-Vertrieb, insbesondere bei der Veräußerung von kapitalintensiven Investitionsgütern wie industriellen Energiesystemen, Großmaschinen oder Enterprise-Software, gleicht kein Einwand dem anderen. Bevor ein Verkäufer argumentativ kontert, muss er verstehen, was sich auf psychologischer Ebene beim Gegenüber abspielt.</p>
    
    <div class="hl hl-blue">
      <strong>Die Ursache von Widerstand: Risiko-Aversion</strong>
      Ein B2B-Entscheider (z. B. technischer Leiter, CFO, Geschäftsführer) kauft nicht nur ein Produkt – er setzt seine teaminterne Reputation, sein Budget und im schlimmsten Fall seinen Arbeitsplatz aufs Spiel. Der Einwand ist daher primär ein unbewusster Schutzmechanismus gegen potenzielles Versagen.
    </div>

    <h3>Der fundamentale Unterschied: Einwand vs. Vorwand</h3>
    <p>Wer einen Vorwand wie einen echten Einwand behandelt, verliert das Gespräch durch informationelle Überfütterung. Ein **Echter Einwand** basiert auf realen, harten Fakten (z. B. unpassende physische Gegebenheiten in der Produktionshalle). Ein **Vorwand** hingegen ist ein emotionales Schutzschild, um die wahre Unsicherheit nicht offenlegen zu müssen.</p>

    <div class="vs-grid">
      <div class="vs-card vs-comp">
        <h4>Vorwand (Emotionales Schutzschild)</h4>
        <ul>
          <li>„Schicken Sie mal Unterlagen, ich schau mir das an.“</li>
          <li>„Wir haben aktuell absolut keine Zeit.“</li>
          <li>„Das Budget ist für dieses Jahr komplett dicht.“</li>
          <li><em>Ziel des Kunden:</em> Höfliche Flucht aus der Verbindlichkeit.</li>
        </ul>
      </div>
      <div class="vs-card vs-realm">
        <h4>Echter Einwand (Reale Barriere)</h4>
        <ul>
          <li>„Unsere Deckenlast in Halle 3 trägt maximal 4 Tonnen.“</li>
          <li>„Die Schnittstelle zu SAP S/4HANA muss zwingend stehen.“</li>
          <li>„Der Aufsichtsrat sperrt Investitionen über 100k bis Q4.“</li>
          <li><em>Ziel des Kunden:</em> Klärung von Machbarkeiten.</li>
        </ul>
      </div>
    </div>
  </div>

  <!-- MODUL 2 -->
  <div class="card">
    <div class="card-title"><span class="ico">⚡</span>Modul 2: Das 4-Stufen-Isolationsmodell im Live-Gespräch</div>
    <p>Um Geisterjagd im Verkaufsgespräch zu vermeiden, wenden Realm-Berater das eiserne Prinzip der **Einwands-Isolation** an. Dadurch wird sichergestellt, dass nach der Entkräftung des Arguments keine neuen Ausflüchte nachgeschoben werden.</p>
    
    <h3>Die 4 Stufen der Isolation</h3>
    <ol>
      <li><strong>Verständnis &amp; Validierung:</strong> Druck aus dem Gespräch nehmen, dem Kunden Recht geben.</li>
      <li><strong>Bedingte Isolationsfrage:</strong> Den Einwand hypothetisch auflösen, um zu sehen, was dahinter liegt.</li>
      <li><strong>Suche nach versteckten Hürden:</strong> Sicherstellen, dass kein zweiter Faktor blockiert.</li>
      <li><strong>Verbindliche Brücke:</strong> Das Gespräch exklusiv auf die Lösung dieser einen Hürde lenken.</li>
    </ol>

    <div class="script-box">
      <div class="script-tag">Wort-für-Wort-Skript: Isolation bei Budget-Blockade</div>
      <p><strong>Kunde:</strong> „Das klingt alles hochspannend, aber wir haben dafür dieses Jahr einfach kein Budget mehr frei.“</p>
      <p><strong>Realm-Berater (Stufe 1):</strong> „Ich verstehe Sie vollkommen, Herr [Name]. Gerade in Zeiten volatiler Märkte hält man die Budgets extrem straff zusammen. Das zeigt einfach, wie verantwortungsvoll Sie wirtschaften.“</p>
      <p><strong>Realm-Berater (Stufe 2 &amp; 3):</strong> „Wenn wir das Thema Budget für einen kurzen Moment komplett ausklammern und so tun, als läge die Freigabe bereits auf Ihrem Tisch... Wäre unser System dann von der Performance und den technischen Kennzahlen her exakt die Lösung, die Sie in Ihrer Produktion haben wollen?“</p>
      <p><strong>Kunde:</strong> „Ja, technisch ist das genau das, was wir brauchen. Aber das Geld ist halt nicht da.“</p>
      <p><strong>Realm-Berater (Stufe 4):</strong> „Verstanden. Das heißt, die Technik passt perfekt, und das einzige Nadelöhr, das uns noch von einer Zusammenarbeit trennt, ist die reine Liquiditäts- und Zahlungsstrukturierung für dieses Kalenderjahr? Wenn wir dafür eine Lösung finden, gehen wir das Projekt gemeinsam an, korrekt?“</p>
    </div>
  </div>

  <div class="nav-btns">
    <div></div>
    <button class="btn btn-primary" onclick="goSec(1)">Weiter zu Modul 3 &amp; 4 →</button>
  </div>
</div>

<!-- ══════════════════════════════ SECTION 1 (M3-M4) ══ -->
<div class="section" id="sec1">
  <div class="sect-progress"><div class="sect-progress-fill" style="width:50%"></div></div>

  <!-- MODUL 3 -->
  <div class="card">
    <div class="card-title"><span class="ico">💎</span>Modul 3: Die Realm Value-Pricing-Strategie (Kosten vs. Investition)</div>
    <p>Wer Investitionsgüter über technische Datenblätter und Preisschilder verkauft, macht sich austauschbar und rutscht unweigerlich in den ruinösen Preiswettbewerb. Spitzenverkäufer rahmen den Preis von Anfang an anders: Sie verkaufen **Wertschöpfung und Risikominimierung**.</p>
    
    <h3>Das mathematische Prinzip der monetären Kontrastierung</h3>
    <p>Ein Preis von 120.000 € für eine industrielle Wärmepumpen-Kaskade wirkt isoliert betrachtet hoch. Setzt man diesen Preis jedoch in Relation zu den kumulierten Verlusten einer verschleppten Modernisierung, schrumpft er psychologisch zusammen.</p>

    <div class="hl hl-amber">
      <strong>Die fundamentale Formel:</strong>
      <p>Investitionspreis &lt; Kosten des aktuellen Zustands (Cost of Inaction) + Wert der neu gewonnenen Effizienz</p>
    </div>

    <h4>Vermeide diese Fehler bei der Preisnennung:</h4>
    <ul>
      <li><strong>Die Entschuldigungshaltung:</strong> „Ich weiß, das ist viel Geld, aber...“ (Zerstört die gefühlte Wertigkeit sofort).</li>
      <li><strong>Das nackte Preisschild:</strong> „Das System kostet 85.000 €.“ ohne direkte Koppelung an die Ertragsseite.</li>
    </ul>
  </div>

  <!-- MODUL 4 -->
  <div class="card">
    <div class="card-title"><span class="ico">📊</span>Modul 4: Die COI-Architektur (Cost of Inaction) &amp; ROI-Kalkulation</div>
    <p>B2B-Entscheider kaufen keine Produkte, sie kaufen Bilanzeffekte. In diesem Modul lernen wir, wie man die *Cost of Inaction* (die Kosten des Nicht-Handelns) so präzise berechnet, dass das Abwarten für den Kunden wirtschaftlich unerträglich wird.</p>

    <h3>Fallstudie: Industrielle Wärmepumpen-Anlage</h3>
    <p>Ein produzierender Betrieb benötigt eine neue thermische Energieversorgung. Die Investition in das hocheffiziente Realm-System beträgt **150.000 €**. Der Mitbewerber bietet ein Altsystem für **100.000 €** an.</p>

    <div class="tbl-wrap">
      <table>
        <thead>
          <tr>
            <th>Kostenfaktor (jährlich)</th>
            <th>Altsystem / Ist-Zustand</th>
            <th>Realm-System</th>
            <th>Realm-Vorteil (jährlich)</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><strong>Energiekosten (Gas/Strom)</strong></td>
            <td>94.000 €</td>
            <td>52.000 €</td>
            <td>+ 42.000 € Ersparnis</td>
          </tr>
          <tr>
            <td><strong>Wartung &amp; CO2-Zertifikate</strong></td>
            <td>18.000 €</td>
            <td>6.000 €</td>
            <td>+ 12.000 € Ersparnis</td>
          </tr>
          <tr>
            <td><strong>Ausfallrisiko (Stillstandszeiten)</strong></td>
            <td>15.000 € (prognostiziert)</td>
            <td>2.000 €</td>
            <td>+ 13.000 € Risikoreduktion</td>
          </tr>
          <tr>
            <td><strong>Gesamteffekt</strong></td>
            <td><strong>127.000 € / Jahr</strong></td>
            <td><strong>60.000 € / Jahr</strong></td>
            <td><strong>+ 67.000 € / Jahr Vorteil</strong></td>
          </tr>
        </tbody>
      </table>
    </div>

    <div class="script-box">
      <div class="script-tag">Wort-für-Wort-Skript: Die COI-Zwinge im Verkaufsgespräch</div>
      <p>„Herr [Name], der Unterschied in der Erstinvestition zwischen dem Standardsystem und unserer Anlage beträgt exakt 50.000 €. Lassen Sie uns das kurz kaufmännisch betrachten: Durch den energetischen Mehrverbrauch und die CO2-Abgaben entstehen Ihnen mit der Standardlösung Mehrkosten von 67.000 € – und das Jahr für Jahr.</p>
      <p>Das bedeutet konkret: **Nach bereits 9 Monaten hat sich der Aufpreis komplett amortisiert.** Wenn Sie die Entscheidung für Realm jetzt um nur ein einziges Quartal verschieben, verbrennen Sie rein rechnerisch knapp 16.750 € an vermeidbaren Betriebskosten, die unwiederbringlich verloren sind. Macht es vor diesem Hintergrund Sinn, mit dem Projektstart auch nur eine Woche länger zu warten?“</p>
    </div>
  </div>

  <div class="nav-btns">
    <button class="btn" onclick="goSec(0)">← Zurück</button>
    <button class="btn btn-primary" onclick="goSec(2)">Weiter zu Modul 5 &amp; 6 →</button>
  </div>
</div>

<!-- ══════════════════════════════ SECTION 2 (M5-M6) ══ -->
<div class="section" id="sec2">
  <div class="sect-progress"><div class="sect-progress-fill" style="width:75%"></div></div>

  <!-- MODUL 5 -->
  <div class="card">
    <div class="card-title"><span class="ico">🎯</span>Modul 5: Abschluss-Trigger &amp; Partnerschaftliche Closing-Techniken</div>
    <p>Ein künstlicher Drucker-Abschluss („Wenn Sie jetzt nicht unterschreiben, verfällt der Rabatt!“) führt im High-Ticket-B2B-Segment unweigerlich zu massiven Stornierungen, rechtlichen Nachspielen und verbrannter Erde. Wir nutzen stattdessen logische und partnerschaftliche Überleitungen.</p>
    
    <h3>Die 3 High-Ticket Closing-Techniken</h3>
    
    <h4>1. Der "Logical Next Step" (Die konsequente Weiterführung)</h4>
    <p>Man fasst die gemeinsam erarbeiteten Fakten zusammen und schlägt den logischen nächsten Schritt als Selbstverständlichkeit vor.</p>
    <div class="hl hl-blue">
      <strong>Skript-Muster:</strong> „Herr [Name], wir haben gemeinsam festgestellt, dass die Anlage technisch perfekt in Ihre Werkshalle passt, der ROI bei unter einem Jahr liegt und Ihr Ingenieursteam voll hinter dem Konzept steht. Der logische nächste Schritt ist nun, dass wir die technische Detailplanung fixieren, damit die Komponenten rechtzeitig zur Jahresrevisionspause im Werk sind. Sollen wir den Liefervertrag auf den 1. oder den 15. des Monats terminieren?“
    </div>

    <h4>2. Die "Risk-Reversal"-Schleife (Vollständige Risikoumkehr)</h4>
    <p>Wenn der Kunde kurz vor dem Ziel zögert, liegt es meist an einer unbewussten Rest-Angst vor einer Fehlentscheidung. Wir nehmen dieses Risiko aktiv auf unsere Schultern.</p>
    <div class="hl hl-blue">
      <strong>Skript-Muster:</strong> „Ich spüre, dass Sie absolut sicher sein wollen, dass die Software-Schnittstelle reibungslos läuft. Lassen Sie uns Folgendes vereinbaren: Wir verankern im Hauptvertrag eine explizite Klausel: Sollte die Datenanbindung innerhalb der ersten 30 Tage nach Live-Gang nicht die vereinbarte Latenz von unter 50ms liefern, haben Sie ein sofortiges Rücktrittsrecht bei voller Kostenerstattung. Wenn wir dieses Risiko komplett für Sie übernehmen – steht unserem gemeinsamen Projektstart dann noch etwas im Wege?“
    </div>
  </div>

  <!-- MODUL 6 -->
  <div class="card">
    <div class="card-title"><span class="ico">🛡️</span>Modul 6: Der Umgang mit unerwarteten Last-Minute-Einwänden</div>
    <p>Es passiert den besten Verkäufern: Alles ist besprochen, der Vertrag liegt auf dem Tisch – und plötzlich wirft der Kunde eine völlig neue Barriere auf. Oft ist dies der sogenannte „Einwand an der Klippe“.</p>

    <h3>Die psychologische Deeskalation</h3>
    <p>Wenn ein Last-Minute-Einwand kommt, darf der Verkäufer niemals emotional reagieren, die Stimme erheben oder in den Verteidigungsmodus gehen. Das signalisiert Unsicherheit.</p>

    <div class="hl hl-red">
      <strong>Die 3-Schritt-Methode für Last-Minute-Einwände:</strong>
      <ol>
        <li><strong>Auffangen:</strong> Den Einwand absolut emotionslos und ruhig spiegeln („Das ist ein absolut berechtigter Punkt, den Sie da ansprechen.“).</li>
        <li><strong>Wertschätzung:</strong> Dem Kunden das Gefühl geben, dass es gut ist, dass er diesen Punkt jetzt anspricht.</li>
        <li><strong>Zurückführen auf das Große Ganze:</strong> Den kleinen Last-Minute-Punkt ins Verhältnis zum bereits bestätigten Gesamt-Mehrwert setzen.</li>
      </ol>
    </div>

    <h4>Szenario: „Ich muss da erst noch einmal eine Nacht drüber schlafen.“</h4>
    <div class="script-box">
      <div class="script-tag">Wort-für-Wort-Skript: Die "Nacht-drüber-schlafen"-Auflösung</div>
      <p><strong>Realm-Berater:</strong> „Das verstehe ich vollkommen. Bei einer Investition dieser Tragweite gehört es zu einer exzellenten Führungskraft dazu, besonnen zu entscheiden. Wenn Sie eine Nacht darüber schlafen – worauf genau wollen Sie Ihren Fokus beim Nachdenken legen? Ist es eher die technische Umsetzung oder die wirtschaftliche Amortisation?“</p>
      <p><strong>Kunde:</strong> „Eigentlich nur, ob mein Team den Umstellungsaufwand nächste Woche neben dem Tagesgeschäft wirklich packt.“</p>
      <p><strong>Realm-Berater:</strong> „Genau um diesen Punkt zu entlasten, stellen wir Ihnen für die ersten 14 Tage einen unserer Implementierungs-Ingenieure exklusiv ins Haus, der die Hauptlast trägt. Ihr Team wird maximal 2 Stunden für die Einweisung benötigt. Wenn wir diesen Punkt also bereits gelöst haben – worüber genau möchten Sie dann heute Nacht schlafen?“</p>
    </div>
  </div>

  <div class="nav-btns">
    <button class="btn" onclick="goSec(1)">← Zurück</button>
    <button class="btn btn-primary" onclick="goSec(3)">Weiter zu Modul 7 &amp; Prüfung →</button>
  </div>
</div>

<!-- ══════════════════════════════ SECTION 3 (M7 + QUIZ) ══ -->
<div class="section" id="sec3">
  <div class="sect-progress"><div class="sect-progress-fill" style="width:100%"></div></div>

  <!-- MODUL 7 -->
  <div class="card">
    <div class="card-title"><span class="ico">📜</span>Modul 7: Die Sign-On-Architektur (Vom 'Ja' zur rechtsgültigen Unterschrift)</div>
    <p>Ein mündliches „Ja“ im Termin ist wertvoll, aber noch kein Umsatz. Die Zeitspanne zwischen dem verbalen Einverständnis und der physischen oder digitalen Signatur (z.B. via DocuSign) ist die gefährlichste Phase im B2B-Vertrieb. Hier schlägt der sogenannte **Kaufreue-Effekt (Buyer's Remorse)** zu.</p>
    
    <h3>Die Absicherung des Abschlusses</h3>
    <ul>
      <li><strong>Keine Zeitfenster offenlassen:</strong> Sätze wie „Ich schicke Ihnen den Vertrag im Laufe der nächsten Woche zu“ sind tödlich. Der Vertrag wird idealerweise noch im Termin vorbereitet oder innerhalb von maximal 2 Stunden digital übermittelt.</li>
      <li><strong>Die administrative Vorbereitung:</strong> Kläre vorab, wer *rechtlich* zeichnungsberechtigt ist. Braucht es eine zweite Unterschrift (Vier-Augen-Prinzip)? Muss der Einkauf oder die Rechtsabteilung noch eine Standardprüfung machen?</li>
      <li><strong>Die Post-Closing-Bestätigung:</strong> Dem Kunden sofort nach dem „Ja“ das Gefühl geben, die absolut richtige Entscheidung getroffen zu haben.</li>
    </ul>

    <div class="hl hl-blue">
      <strong>Skript-Vorlage zur Kaufreue-Prävention:</strong>
      <p>„Herr [Name], Gratulation zu dieser zukunftsorientierten Entscheidung. Sie haben damit heute den Grundstein gelegt, um Ihre Energiekosten im Werk ab dem kommenden Quartal massiv zu senken und die CO2-Strafzahlungen komplett zu eliminieren. Ich werde die Unterlagen nun sofort in unserer Rechtsabteilung finalisieren lassen, sodass Sie diese in ca. 30 Minuten digital in Ihrem Posteingang vorfinden. Sobald Sie kurz gegengezeichnet haben, blockieren wir direkt die Produktions-Slots für Ihre Wärmepumpen, damit wir wie besprochen im Zeitplan bleiben.“</p>
    </div>
  </div>

  <!-- INTENSIVE QUIZ -->
  <div class="quiz-box">
    <h3>⚔️ Realm-Closing-Zertifizierung – Die Abschlussprüfung</h3>
    <div class="qsub">Umfassende Prüfung über alle 7 Module · Nur 100% fehlerfreie Logik führt zum Bestehen.</div>

    <div class="name-row">
      <label for="qename">👤 Name des Teilnehmers:</label>
      <input type="text" id="qename" placeholder="Vor- und Nachname eingeben für das Zertifikat..." autocomplete="name" />
    </div>

    <!-- Q1 -->
    <div class="qitem" id="qq1">
      <div class="qt">1. Ein Kunde äußert im finalen Verkaufsgespräch für eine Industrie-Anlage: „Das System klingt perfekt, aber wir haben aktuell absolut keine Kapazitäten im Team, um uns um die Einführung zu kümmern.“ Wie reagiert der Realm-Closer methodisch korrekt?</div>
      <button class="qopt" onclick="qpick(this,1,'a')"><span class="qdot"></span>Er argumentiert sofort, dass die Einführung gar nicht so lange dauert und man sich nicht so anstellen solle.</button>
      <button class="qopt" onclick="qpick(this,1,'b')"><span class="qdot"></span>Er isoliert den Einwand: „Wenn wir die Kapazitäten für einen Moment ausblenden – gäbe es abgesehen davon einen Grund, warum Sie das System nicht einführen würden?“ Um dann per Hebel zu zeigen, dass die Ineffizienz des aktuellen Zustands die eigentliche Ursache für den Zeitmangel ist.</button>
      <button class="qopt" onclick="qpick(this,1,'c')"><span class="qdot"></span>Er bietet an, das Projekt um 6 Monate zu verschieben, bis das Team wieder mehr Luft hat.</button>
      <div class="qfb ok" id="qfb1ok">✓ Exzellent! Durch die Isolation trennst du den echten Kern von eventuellen Ausflüchten und nutzt danach die "Cost of Inaction"-Logik: Wer keine Zeit hat, muss Ineffizienzen sofort eliminieren, um wieder Zeit zu gewinnen.</div>
      <div class="qfb err" id="qfb1err">✗ Falsch. Option A erzeugt Reaktanz und wirkt arrogant. Option C verschiebt das Problem in eine unendliche Pipeline. Richtig ist B.</div>
    </div>

    <!-- Q2 -->
    <div class="qitem" id="qq2">
      <div class="qt">2. Welches Ziel verfolgt die "Cost of Inaction" (COI) Argumentation in Modul 4?</div>
      <button class="qopt" onclick="qpick(this,2,'a')"><span class="qdot"></span>Dem Kunden zu beweisen, dass die Konkurrenz schlechtere Qualität liefert.</button>
      <button class="qopt" onclick="qpick(this,2,'b')"><span class="qdot"></span>Dem Kunden mathematisch schwarz auf weiß vor Augen zu führen, dass das Beibehalten des aktuellen Zustands pro Monat teurer ist als die Investitions- und Amortisationsrate des neuen Systems.</button>
      <button class="qopt" onclick="qpick(this,2,'c')"><span class="qdot"></span>Den Preis des Produkts künstlich aufzublähen, um mehr Marge zu erzielen.</button>
      <div class="qfb ok" id="qfb2ok">✓ Perfekt! B2B-Entscheider handeln nach Zahlen, Daten und Fakten. Wenn das Abwarten jeden Monat 5.000 € kostet, das System aber nur eine Leasingrate von 2.500 € aufruft, ist der Nicht-Kauf eine aktive Geldverbrennung.</div>
      <div class="qfb err" id="qfb2err">✗ Falsch. COI hat nichts mit dem Schlechtreden von Konkurrenten zu tun und dient auch nicht der Margen-Aufblähung. Es ist die reine betriebswirtschaftliche Logik des Ist-Zustands. Richtig ist B.</div>
    </div>

    <!-- Q3 -->
    <div class="qitem" id="qq3">
      <div class="qt">3. Sie sind am Ende der Präsentation. Der Kunde hat alle Mehrwerte bestätigt, zögert nun aber schweigend vor dem Vertragsentwurf. Welche Closing-Technik ist anzuwenden?</div>
      <button class="qopt" onclick="qpick(this,3,'a')"><span class="qdot"></span>Die "Logical Next Step"-Frage formulieren und die administrative Umsetzung (z.B. Lieferzeitfenster oder technischer Kick-off) vorschlagen.</button>
      <button class="qopt" onclick="qpick(this,3,'b')"><span class="qdot"></span>Aggressiven Druck aufbauen: „Wenn Sie jetzt nicht unterschreiben, ist die Anlage weg.“</button>
      <button class="qopt" onclick="qpick(this,3,'c')"><span class="qdot"></span>Das Schweigen aussitzen und den Kunden so lange anstarren, bis er aus Unbehagen von selbst unterschreibt.</button>
      <div class="qfb ok" id="qfb3ok">✓ Großartig! Im gehobenen B2B-Segment führt man den Kunden elegant über die administrative Schwelle. Der "Logical Next Step" wirkt vollkommen natürlich und partnerschaftlich.</div>
      <div class="qfb err" id="qfb3err">✗ Falsch. Druck (B) zerstört das Vertrauen im B2B sofort. Das reine psychologische Anschweigen (C) kann in manchen Consumer-Märkten funktionieren, wirkt bei professionellen Geschäftsführern jedoch plump. Richtig ist A.</div>
    </div>

    <!-- Q4 -->
    <div class="qitem" id="qq4">
      <div class="qt">4. Was versteht man unter dem Begriff "Buyer's Remorse" in Modul 7 und wie verhindert man ihn aktiv?</div>
      <button class="qopt" onclick="qpick(this,4,'a')"><span class="qdot"></span>Die Reue des Verkäufers, das Produkt zu billig abgegeben zu haben. Man verhindert sie durch nachträgliche Preiserhöhungen.</button>
      <button class="qopt" onclick="qpick(this,4,'b')"><span class="qdot"></span>Den Kaufreue-Effekt des Kunden direkt nach dem verbalen 'Ja'. Man verhindert ihn durch sofortige digitale Übermittlung des Vertrags und eine Bestätigung der strategischen Vorteile (Post-Closing).</button>
      <button class="qopt" onclick="qpick(this,4,'c')"><span class="qdot"></span>Ein juristischer Begriff für Mängelgewährleistung.</div>
      <div class="qfb ok" id="qfb4ok">✓ Absolut korrekt! Sobald der Kunde „Ja“ sagt, beginnt sein Gehirn oft, Risiken hochzurechnen. Wer hier tagelang mit dem Vertrag wartet, riskiert, dass der Deal intern gecancelt wird. Schnelligkeit und mentale Bestätigung sichern den Erfolg.</div>
      <div class="qfb err" id="qfb4err">✗ Falsch. Buyer's Remorse betrifft immer den Käufer, der kurz nach der Entscheidung kalte Füße bekommt. Antwort B ist der einzige professionelle Schutzmechanismus.</div>
    </div>

    <!-- SCORE BOX -->
    <div class="quiz-score" id="qscorebox">
      <div class="qs-val" id="qscoreval">0 / 4</div>
      <div class="qs-lbl" id="qscorelbl">Prüfungsergebnis</div>
      <div id="qscoretext" style="margin-top:10px; font-weight:700; font-size:15px"></div>
    </div>
  </div>

  <!-- FOOTER NAV -->
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
const correctAnswers = { 1: 'b', 2: 'b', 3: 'a', 4: 'b' };

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
    
    if(score === 4) {
      scoreText.innerHTML = `🏆 Herausragend, ${name}! Du hast die Value-Closing Zertifizierung mit der Bestnote von 100% BESTANDEN! Du bist nun offiziell qualifiziert, komplexe B2B-Deals auf Enterprise-Niveau souverän abzuschließen.`;
      scoreText.style.color = "var(--green-dark)";
    } else if(score >= 3) {
      scoreText.innerHTML = `🎉 Gut gemacht, ${name}! Du hast die Prüfung bestanden. Schau dir die verfehlten Punkte noch einmal kurz an, um die absolute Perfektion zu erreichen.`;
      scoreText.style.color = "var(--green-mid)";
    } else {
      scoreText.innerHTML = `⚠️ Zertifizierung nicht bestanden, ${name}. Für das High-Ticket Segment müssen die psychologischen Mechanismen fehlerfrei sitzen. Setze die Abschnitte zurück und versuche es erneut!`;
      scoreText.style.color = "var(--red)";
    }
  }
}
</script>
</body>
</html>
