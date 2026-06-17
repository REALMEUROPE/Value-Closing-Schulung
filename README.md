<!DOCTYPE html>
<html lang="de">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Realm Germany – B2B Sales Masterclass</title>
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
body{font-family:-apple-system,BlinkMacSystemFont,'Segoe UI',Roboto,sans-serif;background:#F4F5F7;color:#1A1A1A;min-height:100vh;padding:1.5rem 1rem}
.wrapper{max-width:780px;margin:0 auto}
.main-header{background:linear-gradient(135deg,#0B3D6B 0%,#1A6B4A 100%);border-radius:14px;padding:2rem;margin-bottom:1.5rem;color:#fff}
.main-header .eyebrow{font-size:11px;letter-spacing:2px;text-transform:uppercase;opacity:.7;margin-bottom:6px}
.main-header h1{font-size:24px;font-weight:700;margin-bottom:4px}
.main-header p{font-size:13px;opacity:.8;margin-bottom:1rem}
.header-meta{display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:8px;font-size:12px;opacity:.8}
.hprog{background:rgba(255,255,255,.2);border-radius:8px;height:7px;margin-top:10px}
.hprog-fill{background:#fff;border-radius:8px;height:7px;width:0%;transition:width .5s}
.mod-nav{display:grid;grid-template-columns:repeat(auto-fill,minmax(140px,1fr));gap:10px;margin-bottom:1.5rem}
.nav-btn{background:#fff;border:1px solid #E5E7EB;border-radius:12px;padding:.875rem 1rem;cursor:pointer;text-align:left;transition:all .2s;position:relative}
.nav-btn:hover{border-color:#9CA3AF;background:#F9FAFB}
.nav-btn.active{border:2px solid #1A6B4A;background:#F0FDF4}
.nav-btn.done{border-color:#059669}
.nav-btn .nicon{font-size:20px;margin-bottom:6px}
.nav-btn .ntitle{font-size:12px;font-weight:700;color:#374151}
.nav-btn .nsub{font-size:11px;color:#6B7280;margin-top:2px}
.nav-btn .ncheck{font-size:11px;color:#059669;font-weight:600;margin-top:4px}
.card{background:#fff;border:1px solid #E5E7EB;border-radius:14px;padding:1.75rem;margin-bottom:1.25rem}
.module{display:none}
.module.active{display:block}
.mod-title{font-size:20px;font-weight:700;margin-bottom:1rem;display:flex;align-items:center;gap:10px;color:#0B3D6B}
.mod-title .mico{font-size:22px}
h3{font-size:15px;font-weight:700;margin:1.25rem 0 .5rem;color:#1A1A1A}
h4{font-size:14px;font-weight:700;margin:.875rem 0 .3rem;color:#0B3D6B}
p{font-size:14px;line-height:1.7;color:#374151;margin-bottom:.6rem}
li{font-size:14px;line-height:1.7;color:#374151;margin-bottom:.3rem}
ul,ol{padding-left:1.25rem;margin-bottom:.75rem}
.highlight{background:#F0FDF4;border-left:3px solid #059669;padding:.75rem 1rem;border-radius:0 10px 10px 0;margin:.875rem 0;font-size:13.5px;line-height:1.6;color:#1A1A1A}
.hl-amber{background:#FFFBEB;border-left:3px solid #F59E0B;padding:.75rem 1rem;border-radius:0 10px 10px 0;margin:.875rem 0;font-size:13.5px;line-height:1.6;color:#1A1A1A}
.hl-blue{background:#EFF6FF;border-left:3px solid #3B82F6;padding:.75rem 1rem;border-radius:0 10px 10px 0;margin:.875rem 0;font-size:13.5px;line-height:1.6;color:#1A1A1A}
.hl-red{background:#FEF2F2;border-left:3px solid #DC2626;padding:.75rem 1rem;border-radius:0 10px 10px 0;margin:.875rem 0;font-size:13.5px;line-height:1.6;color:#1A1A1A}
.stat-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(130px,1fr));gap:10px;margin:1rem 0}
.stat{background:#F8F9FA;border-radius:10px;padding:1rem;text-align:center}
.stat .val{font-size:22px;font-weight:700;color:#1A6B4A}
.stat .lbl{font-size:11px;color:#6B7280;margin-top:4px;line-height:1.4}
.tbl-wrap{overflow-x:auto;margin:.875rem 0}
table{width:100%;border-collapse:collapse;font-size:13px}
th{background:#F3F4F6;padding:8px 12px;text-align:left;font-weight:700;border-bottom:1px solid #E5E7EB;color:#374151}
td{padding:8px 12px;border-bottom:1px solid #F3F4F6;color:#4B5563;vertical-align:top}
tr:last-child td{border-bottom:none}
tr:hover td{background:#FAFAFA}
.badge{display:inline-block;padding:2px 9px;border-radius:12px;font-size:11px;font-weight:700}
.bg{background:#D1FAE5;color:#065F46}
.bb{background:#DBEAFE;color:#1E40AF}
.ba{background:#FEF3C7;color:#92400E}
.br{background:#FEE2E2;color:#991B1B}
.steps{margin:.875rem 0}
.step{display:flex;gap:12px;margin-bottom:.875rem;align-items:flex-start}
.step-num{width:28px;height:28px;border-radius:50%;background:#1A6B4A;color:#fff;font-size:13px;font-weight:700;display:flex;align-items:center;justify-content:center;flex-shrink:0;margin-top:2px}
.step-body h4{font-size:14px;font-weight:700;margin-bottom:2px;color:#1A1A1A}
.step-body p{font-size:13px;color:#6B7280;margin:0}
.nav-btns{display:flex;justify-content:space-between;margin-top:1.5rem;gap:10px}
.btn{padding:.65rem 1.25rem;border-radius:10px;border:1px solid #D1D5DB;background:#fff;cursor:pointer;font-size:14px;font-weight:600;color:#374151;transition:all .2s;display:inline-flex;align-items:center;gap:6px}
.btn:hover{background:#F9FAFB;border-color:#9CA3AF}
.btn-primary{background:#1A6B4A;color:#fff;border-color:#1A6B4A}
.btn-primary:hover{background:#155C3E}
.btn-primary:disabled{background:#9CA3AF;border-color:#9CA3AF;cursor:not-allowed}
.skript-box{background:#F8F9FA;border:1px solid #E5E7EB;border-radius:12px;padding:1.25rem;margin:.875rem 0}
.skript-box .sk-label{font-size:10px;font-weight:700;text-transform:uppercase;letter-spacing:1.5px;color:#059669;margin-bottom:.5rem;display:flex;align-items:center;gap:6px}
.skript-box .sk-text{font-size:13.5px;color:#1A1A1A;line-height:1.75;font-style:italic;border-left:3px solid #1A6B4A;padding-left:.875rem}
.skript-box .sk-note{font-size:12px;color:#6B7280;margin-top:.5rem;font-style:normal}
.vs-grid{display:grid;grid-template-columns:1fr 1fr;gap:12px;margin:1rem 0}
.vs-card{border-radius:12px;padding:1.1rem;border:2px solid transparent}
.vs-good{background:#F0FDF4;border-color:#059669}
.vs-bad{background:#FEF2F2;border-color:#FCA5A5}
.vs-card h4{font-size:13px;font-weight:700;margin-bottom:.5rem}
.vs-card p{font-size:13px;margin:0}
.framework-steps{margin:1rem 0}
.fw-step{display:flex;gap:14px;margin-bottom:1rem;align-items:flex-start;background:#F9FAFB;border-radius:10px;padding:.875rem 1rem;border:1px solid #F3F4F6}
.fw-num{width:32px;height:32px;border-radius:50%;background:linear-gradient(135deg,#0B3D6B,#1A6B4A);color:#fff;font-size:13px;font-weight:700;display:flex;align-items:center;justify-content:center;flex-shrink:0}
.fw-body h4{font-size:14px;font-weight:700;margin-bottom:3px;color:#0B3D6B}
.fw-body p{font-size:13px;color:#374151;margin:0}
.email-box{background:#F8F9FA;border:1px solid #E5E7EB;border-radius:12px;padding:1.25rem;margin:.875rem 0}
.email-box .email-header{font-size:11px;font-weight:700;text-transform:uppercase;letter-spacing:1px;color:#6B7280;margin-bottom:.75rem;padding-bottom:.5rem;border-bottom:1px solid #E5E7EB}
.email-box .email-subject{font-size:13px;font-weight:700;color:#1A1A1A;margin-bottom:.75rem}
.email-box .email-body{font-size:13px;color:#374151;line-height:1.75;white-space:pre-line}
.kpi-box{background:linear-gradient(135deg,#F0FDF4,#EFF6FF);border:1px solid #D1FAE5;border-radius:12px;padding:1.25rem;margin:.875rem 0}
.kpi-row{display:flex;align-items:center;justify-content:space-between;padding:.5rem 0;border-bottom:1px solid rgba(0,0,0,.06)}
.kpi-row:last-child{border-bottom:none}
.kpi-label{font-size:13px;color:#374151}
.kpi-val{font-size:14px;font-weight:700;color:#1A6B4A}
.aufgabe-box{background:#EFF6FF;border:1px solid #BFDBFE;border-radius:12px;padding:1.25rem;margin-top:1.25rem}
.aufgabe-box h4{font-size:13px;font-weight:700;color:#1D4ED8;margin-bottom:.5rem;display:flex;align-items:center;gap:6px}
.aufgabe-box ol{padding-left:1.2rem;margin:0}
.aufgabe-box li{font-size:13px;color:#1E3A5F;margin-bottom:.4rem}
.mquiz{background:#F8F9FA;border:1px solid #E5E7EB;border-radius:12px;padding:1.25rem;margin-top:1.25rem}
.mquiz h4{font-size:14px;font-weight:700;margin-bottom:.5rem;color:#0B3D6B}
.mquiz .qtext{font-size:13px;color:#4B5563;margin-bottom:.75rem}
.mopt{display:flex;align-items:flex-start;gap:8px;background:#fff;border:1px solid #E5E7EB;border-radius:9px;padding:.6rem .875rem;cursor:pointer;margin-bottom:6px;font-size:13px;color:#374151;line-height:1.5;transition:all .15s;width:100%;text-align:left}
.mopt:hover{border-color:#9CA3AF;background:#F9FAFB}
.mopt .dot{width:14px;height:14px;border:2px solid #D1D5DB;border-radius:50%;flex-shrink:0;margin-top:2px}
.mopt.correct{background:#ECFDF5;border-color:#059669;color:#065F46}
.mopt.correct .dot{background:#059669;border-color:#059669}
.mopt.wrong{background:#FEF2F2;border-color:#DC2626;color:#7F1D1D}
.mopt.wrong .dot{background:#DC2626;border-color:#DC2626}
.mfb{display:none;font-size:12px;line-height:1.6;padding:.6rem .875rem;border-radius:8px;margin-top:.5rem}
.mfb.show{display:block}
.mfb.ok{background:#ECFDF5;color:#065F46;border:1px solid #A7F3D0}
.mfb.err{background:#FEF2F2;color:#7F1D1D;border:1px solid #FECACA}
.name-row{display:flex;align-items:center;gap:12px;background:#F8F9FA;border:1px solid #E5E7EB;border-radius:10px;padding:.875rem 1rem;margin-bottom:1.5rem}
.name-row label{font-size:14px;font-weight:700;white-space:nowrap;color:#1A6B4A}
.name-row input{flex:1;border:none;background:transparent;font-size:14px;color:#1A1A1A;outline:none}
.name-row input::placeholder{color:#9CA3AF}
.prog-wrap{margin-bottom:1.5rem}
.prog-meta{display:flex;justify-content:space-between;font-size:12px;color:#6B7280;margin-bottom:6px}
.prog-bar{background:#E5E7EB;border-radius:8px;height:6px}
.prog-fill{background:#1A6B4A;border-radius:8px;height:6px;width:0%;transition:width .4s}
.qblock{padding:1.25rem 0;border-bottom:1px solid #F3F4F6}
.qblock:last-of-type{border-bottom:none;padding-bottom:0}
.qblock:first-of-type{padding-top:0}
.q-header{display:flex;align-items:center;gap:10px;margin-bottom:.5rem}
.q-num{font-size:13px;font-weight:700;color:#374151}
.bdg{display:inline-block;padding:2px 9px;border-radius:12px;font-size:10px;font-weight:700;text-transform:uppercase;letter-spacing:.3px}
.bdg-h{background:#FEE2E2;color:#991B1B}
.bdg-m{background:#FEF3C7;color:#92400E}
.qtext{font-size:14px;font-weight:600;line-height:1.6;color:#1A1A1A;margin-bottom:.75rem}
.opt{display:flex;align-items:flex-start;gap:10px;background:#fff;border:1px solid #E5E7EB;border-radius:10px;padding:.65rem 1rem;cursor:pointer;margin-bottom:6px;font-size:13px;color:#374151;line-height:1.5;transition:all .15s;width:100%;text-align:left}
.opt:hover{border-color:#9CA3AF;background:#F9FAFB}
.opt .dot{width:16px;height:16px;border:2px solid #D1D5DB;border-radius:50%;flex-shrink:0;margin-top:2px;transition:all .15s}
.opt.correct{background:#ECFDF5;border-color:#059669;color:#065F46}
.opt.correct .dot{background:#059669;border-color:#059669}
.opt.wrong{background:#FEF2F2;border-color:#DC2626;color:#7F1D1D}
.opt.wrong .dot{background:#DC2626;border-color:#DC2626}
.opt.locked{pointer-events:none}
.fb{display:none;font-size:12px;line-height:1.6;padding:.6rem .875rem;border-radius:8px;margin-top:.5rem}
.fb.show{display:block}
.fb.ok{background:#ECFDF5;color:#065F46;border:1px solid #A7F3D0}
.fb.err{background:#FEF2F2;color:#7F1D1D;border:1px solid #FECACA}
.score-box{display:none;background:#F9FAFB;border:1px solid #E5E7EB;border-radius:14px;padding:2rem;text-align:center;margin-top:1.5rem}
.score-box.show{display:block}
.score-val{font-size:52px;font-weight:700;color:#1A6B4A;line-height:1}
.score-val.fail{color:#DC2626}
.score-pct{font-size:14px;color:#6B7280;margin-top:4px}
.score-verdict{display:inline-block;margin:1rem 0 .5rem;padding:6px 22px;border-radius:20px;font-size:14px;font-weight:700;letter-spacing:.5px}
.vpass{background:#D1FAE5;color:#065F46}
.vfail{background:#FEE2E2;color:#991B1B}
.score-comment{font-size:14px;color:#374151;margin-bottom:1.25rem}
.missed-wrap{text-align:left;margin:1rem 0 1.5rem}
.missed-title{font-size:13px;font-weight:700;margin-bottom:.5rem;color:#374151}
.missed-item{font-size:12px;color:#6B7280;padding:3px 0 3px 20px;position:relative}
.missed-item::before{content:"✗";color:#DC2626;position:absolute;left:0}
.btn-row{display:flex;gap:10px;justify-content:center;flex-wrap:wrap}
.mail-note{font-size:12px;color:#DC2626;margin-top:.75rem;min-height:16px;text-align:center}
.mail-ok{color:#059669!important}
.footer{text-align:center;font-size:11px;color:#9CA3AF;margin-top:2rem;padding-bottom:1rem}
@media(max-width:520px){
  .card{padding:1.25rem}
  .main-header{padding:1.5rem 1.25rem}
  .score-val{font-size:40px}
  .mod-nav{grid-template-columns:repeat(2,1fr)}
  .vs-grid{grid-template-columns:1fr}
}
</style>
</head>
<body>
<div class="wrapper">

<div class="main-header">
  <div class="eyebrow">Realm Germany GmbH · B2B Sales Masterclass 2025</div>
  <h1>High-Ticket B2B Vertrieb – Komplette Schulung</h1>
  <p>Einwandbehandlung · Closing · Key Account Management · Preisverhandlung · Pipeline</p>
  <div class="header-meta">
    <span id="h-mod-txt">Modul 1 von 8</span>
    <span id="h-prog-txt">0 % abgeschlossen</span>
  </div>
  <div class="hprog"><div class="hprog-fill" id="hprog"></div></div>
</div>

<div class="mod-nav">
  <button class="nav-btn active" id="nc0" onclick="showMod(0)"><div class="nicon">🧠</div><div class="ntitle">Modul 1</div><div class="nsub">Einwand vs. Vorwand</div></button>
  <button class="nav-btn" id="nc1" onclick="showMod(1)"><div class="nicon">⚙️</div><div class="ntitle">Modul 2</div><div class="nsub">LAEV-Framework</div></button>
  <button class="nav-btn" id="nc2" onclick="showMod(2)"><div class="nicon">⚔️</div><div class="ntitle">Modul 3</div><div class="nsub">Die 3 Top-Einwände</div></button>
  <button class="nav-btn" id="nc3" onclick="showMod(3)"><div class="nicon">🎯</div><div class="ntitle">Modul 4</div><div class="nsub">Closing-Frameworks</div></button>
  <button class="nav-btn" id="nc4" onclick="showMod(4)"><div class="nicon">👻</div><div class="ntitle">Modul 5</div><div class="nsub">Anti-Ghosting</div></button>
  <button class="nav-btn" id="nc5" onclick="showMod(5)"><div class="nicon">📈</div><div class="ntitle">Modul 6</div><div class="nsub">Key Account &amp; Upsell</div></button>
  <button class="nav-btn" id="nc6" onclick="showMod(6)"><div class="nicon">🛡️</div><div class="ntitle">Modul 7</div><div class="nsub">Preisverhandlung</div></button>
  <button class="nav-btn" id="nc7" onclick="showMod(7)"><div class="nicon">🏆</div><div class="ntitle">Abschlusstest</div><div class="nsub">20 Fragen</div></button>
</div>

<!-- ══════════════════ MODULE 0: EINWAND vs. VORWAND ══ -->
<div class="module active" id="m0">
<div class="card">
  <div class="mod-title"><span class="mico">🧠</span>Das Mindset – Einwand vs. Vorwand</div>
  <p>Bevor wir über Skripte sprechen, müssen wir das Mindset kalibrieren. Ein Einwand im High-Ticket-Bereich ist kein „Nein" zum Produkt, sondern ein <strong>Hilferuf nach mehr Sicherheit</strong>. Wer 50.000–500.000 €+ investiert, hat massive Angst, eine Fehlentscheidung zu treffen, seinen Job zu riskieren oder intern als Treiber eines gescheiterten Projekts zu gelten.</p>

  <h3>Die Psychologie hinter dem Einwand</h3>
  <p>Stell dir vor, du bist Einkaufsleiter in einem mittelständischen Industrieunternehmen. Dein Vorstand erwartet Kosteneinsparungen. Du sitzt einem Vertriebler gegenüber und sein Angebot klingt vielversprechend – aber es ist teuer. Du weißt nicht, ob die Technik wirklich hält was sie verspricht. Du weißt nicht, wie dein CFO reagiert. Du weißt nicht, ob die IT mitspielen wird. Was sagst du?</p>
  <p>Du sagst: <strong>„Das Budget ist aktuell eingefroren."</strong> – Weil das sicher ist. Weil es höflich ist. Weil es dich nicht angreifbar macht. Das ist der Vorwand.</p>
  <div class="hl-blue"><strong>Entscheider-Psychologie:</strong> Je größer das Investment, desto stärker ist die Angst vor dem persönlichen Risiko. B2B-Entscheider kaufen oft nicht das beste Produkt – sie kaufen das Produkt, das sie am besten intern verteidigen können. Deine Aufgabe: Ihnen diese Verteidigungsmunition liefern.</div>

  <h3>Einwand vs. Vorwand – die entscheidende Unterscheidung</h3>
  <div class="tbl-wrap"><table>
    <thead><tr><th>Merkmal</th><th>Echter Einwand</th><th>Vorwand</th></tr></thead>
    <tbody>
      <tr><td><strong>Definition</strong></td><td>Ein reales Hindernis, das den Kauf tatsächlich blockiert</td><td>Ein vorgeschobener Grund, der den wahren Einwand verdeckt</td></tr>
      <tr><td><strong>Reaktion auf Isolationsfrage</strong></td><td>„Nein, das ist der einzige Grund."</td><td>„Na ja, da wäre noch..."</td></tr>
      <tr><td><strong>Typische Beispiele</strong></td><td>Budget wirklich nicht genehmigt, technische Inkompatibilität, Entscheider ist nicht erreichbar</td><td>„Keine Zeit", „zu teuer" (wenn ROI nicht verstanden), „kein Bedarf" (wenn Schmerz nicht gespürt)</td></tr>
      <tr><td><strong>Richtige Reaktion</strong></td><td>Sofort mit LAEV behandeln</td><td>Zuerst entlarven, dann den echten Einwand behandeln</td></tr>
      <tr><td><strong>Fehler</strong></td><td>Zu früh lösen ohne Isolation</td><td>Den Vorwand für bare Münze nehmen und behandeln</td></tr>
    </tbody>
  </table></div>

  <h3>Die Isolations-Methode – die wichtigste Frage der Schulung</h3>
  <p>Diese eine Frage rettet mehr Deals als jedes Closing-Skript. Sie zwingt den Kunden, ehrlich zu sein – und sie wirkt, weil sie nicht konfrontativ, sondern kooperativ formuliert ist.</p>
  <div class="skript-box">
    <div class="sk-label">💬 Skript: Die universelle Isolationsfrage</div>
    <div class="sk-text">„Herr/Frau [Name], einmal angenommen, das Budget wäre für diesen Moment gar kein Thema und vollkommen freigegeben... gäbe es dann noch einen anderen Grund, warum wir das Projekt nicht gemeinsam umsetzen?"</div>
    <div class="sk-note">→ Danach: Schweigen. Mindestens 3–5 Sekunden. Die Stille ist unangenehm – für dich und für den Kunden. Wer zuerst spricht, verliert. Warte auf die Antwort.</div>
  </div>

  <h3>Die zwei möglichen Reaktionen und was sie bedeuten</h3>
  <div class="vs-grid">
    <div class="vs-card vs-good">
      <h4>✅ Szenario A – Echter Einwand identifiziert</h4>
      <p>Kunde: <em>„Nein, wenn das Budget freigegeben wäre, würden wir es sofort machen."</em><br><br>→ Glückwunsch! Das Budget ist das einzige Hindernis. Jetzt lohnt es sich, mit konkreten Finanzierungsoptionen oder dem Cost-of-Inaction-Argument zu arbeiten.</p>
    </div>
    <div class="vs-card vs-bad">
      <h4>⚠️ Szenario B – Vorwand entlarvt</h4>
      <p>Kunde: <em>„Na ja, ich müsste trotzdem noch sehen, ob unsere IT die Schnittstellen freigibt."</em><br><br>→ Das Budget war vorgeschoben! Behandle zuerst die IT-Frage. Wenn du eine Finanzierungslösung anbietest, ohne das IT-Problem zu klären, ist der Deal trotzdem tot.</p>
    </div>
  </div>

  <h3>Die 6 häufigsten Vorwände im B2B – und was dahintersteckt</h3>
  <div class="tbl-wrap"><table>
    <thead><tr><th>Der Vorwand</th><th>Was wirklich dahintersteckt</th><th>Dein nächster Schritt</th></tr></thead>
    <tbody>
      <tr><td>„Das Budget ist eingefroren."</td><td>Angst vor interner Ablehnung / ROI nicht verstanden / kein Budget-Champion</td><td>Isolationsfrage stellen</td></tr>
      <tr><td>„Wir haben aktuell keine Zeit."</td><td>Kein gesehener Urgency / Implementierungsangst</td><td>Cost of Inaction berechnen</td></tr>
      <tr><td>„Wir prüfen das noch intern."</td><td>Interner Widerstand / Entscheider hat keine Kompetenz / Konkurrenz im Rennen</td><td>Champion identifizieren und stärken</td></tr>
      <tr><td>„Schicken Sie uns erstmal ein Angebot."</td><td>Kein Termin geplant / Deal wird begraben</td><td>No-Offer-Without-Date einsetzen</td></tr>
      <tr><td>„Wir sind mit unserem aktuellen Anbieter zufrieden."</td><td>Wechselbarriere zu hoch / Benchmark fehlt</td><td>Proof-of-Concept / Benchmark-Taktik</td></tr>
      <tr><td>„Das ist zu teuer."</td><td>ROI nicht klar / Vergleich mit falschem Wettbewerber</td><td>ROI-Umdrehung: TCO vs. Anschaffung</td></tr>
    </tbody>
  </table></div>

  <h3>Das Mindset des Hochleistungs-Vertriebs</h3>
  <p>Die besten B2B-Vertriebler betrachten jeden Einwand als <strong>wertvolle Information</strong>, nicht als Angriff. Jeder Einwand zeigt dir, wo der Kunde noch unsicher ist. Deine Reaktion entscheidet, ob er sich verstanden oder angegriffen fühlt – und damit, ob er sich öffnet oder zumacht.</p>
  <div class="stat-grid">
    <div class="stat"><div class="val">60%</div><div class="lbl">aller Einwände sind Vorwände – der echte Grund liegt woanders</div></div>
    <div class="stat"><div class="val">2–3x</div><div class="lbl">höhere Abschlussquote durch Isolation vor Behandlung</div></div>
    <div class="stat"><div class="val">3–5s</div><div class="lbl">Schweigen nach der Isolationsfrage erzeugt maximale Ehrlichkeit</div></div>
    <div class="stat"><div class="val">150k€+</div><div class="lbl">ab dieser Investitionssumme steigt Vorwand-Häufigkeit auf über 80%</div></div>
  </div>

  <div class="aufgabe-box">
    <h4>📝 Praxis-Übung (5 Min.)</h4>
    <ol>
      <li>Denk an deinen letzten Deal, der verloren gegangen ist. Was war der genannte Grund? War es ein echter Einwand oder ein Vorwand?</li>
      <li>Schreibe den Vorwand auf – und daneben: Was war wahrscheinlich der echte Hinderungsgrund?</li>
      <li>Übe die Isolationsfrage laut vor dem Spiegel. Sie muss locker und gesprächsweise klingen, nicht wie eine Verhörfrage.</li>
    </ol>
  </div>

  <div class="mquiz">
    <h4>🎯 Quick-Check</h4>
    <div class="qtext">Ein Kunde sagt: „Das Budget ist eingefroren." Du fragst mit der Isolationsfrage nach. Er antwortet: „Naja, eigentlich müsste auch noch die Rechtsabteilung zustimmen." Was bedeutet das?</div>
    <button class="mopt" onclick="mqPick(this,'m0q1','a')"><span class="dot"></span>Das Budget ist der echte Einwand – Finanzierungslösung anbieten</button>
    <button class="mopt" onclick="mqPick(this,'m0q1','b')"><span class="dot"></span>Das Budget war ein Vorwand – der echte Einwand ist die Rechtsabteilung</button>
    <button class="mopt" onclick="mqPick(this,'m0q1','c')"><span class="dot"></span>Es gibt zwei Einwände – beide gleichzeitig behandeln</button>
    <div class="mfb ok" id="mq-m0q1-ok">✓ Richtig! Das Budget war vorgeschoben. Den Einwand „Rechtsabteilung" zuerst lösen – sonst nützt dir die beste Finanzierungslösung gar nichts.</div>
    <div class="mfb err" id="mq-m0q1-err">✗ Die Isolationsfrage hat den Vorwand entlarvt. Das Budget war nicht der echte Grund – behandle immer zuerst den echten Einwand: die Rechtsabteilung.</div>
  </div>
  <div class="nav-btns"><div></div><button class="btn btn-primary" onclick="nextMod(0)">Weiter: LAEV-Framework →</button></div>
</div>
</div>

<!-- ══════════════════ MODULE 1: LAEV FRAMEWORK ══ -->
<div class="module" id="m1">
<div class="card">
  <div class="mod-title"><span class="mico">⚙️</span>Das L-A-E-V-Framework – Professionelle Einwandbehandlung</div>
  <p>Egal, welcher Einwand kommt: Wir schlagen nicht verbal zurück – wir <strong>fangen den Kunden auf</strong>. Das LAEV-Framework ist der 4-Schritt-Prozess, der jeden Einwand professionell entschärft und in einen Abschluss umwandelt. Es ist kein starres Skript – es ist eine Denkstruktur, die du für jeden Einwand flexibel einsetzen kannst.</p>

  <h3>Warum die Reihenfolge entscheidend ist</h3>
  <p>Die meisten Vertriebsanfänger machen denselben Fehler: Sie hören einen Einwand und springen sofort zur Lösung. Das fühlt sich für sie effizient an. Für den Kunden fühlt es sich an wie: „Der hat mich gar nicht zugehört." Das Ergebnis ist erhöhte Abwehr statt Offenheit. Das LAEV-Framework zwingt dich, zuerst den Boden zu bereiten – bevor du säst.</p>

  <div class="framework-steps">
    <div class="fw-step">
      <div class="fw-num">L</div>
      <div class="fw-body">
        <h4>Lauschen & Atmen – Die 2-Sekunden-Regel</h4>
        <p>Lass den Kunden vollständig ausreden. Mach danach eine bewusste Pause von 2–3 Sekunden. Diese Pause signalisiert: „Ich nehme das ernst und denke wirklich darüber nach." Wer sofort kontert, wirkt wie ein vorbereiteter Drücker, dem die Antwort egal war. Die 2-Sekunden-Pause kostet dich nichts – und gewinnt dir Vertrauen.</p>
        <p style="font-size:12px;color:#6B7280;margin-top:.4rem">Übung: Zähle beim nächsten Einwand innerlich bis 3, bevor du antwortest. Es wird sich unnatürlich anfühlen – das ist normal.</p>
      </div>
    </div>
    <div class="fw-step">
      <div class="fw-num">A</div>
      <div class="fw-body">
        <h4>Anerkennen & Validieren – Druck rausnehmen</h4>
        <p>Nimm den Druck aus der Situation. Gib dem Kunden recht in seiner <em>Wahrnehmung</em>, nicht in der Sache selbst. Der Unterschied ist entscheidend: Du bestätigst, dass sein Gefühl berechtigt ist – nicht, dass sein Einwand faktisch korrekt ist.</p>
        <div class="vs-grid" style="margin-top:.75rem">
          <div class="vs-card vs-good">
            <h4>✅ Richtige Validierung</h4>
            <p>„Ich kann absolut nachvollziehen, dass Sie bei einer Investition in dieser Größenordnung genau hinschauen müssen – das wäre bei mir genauso."</p>
          </div>
          <div class="vs-card vs-bad">
            <h4>❌ Falsche Validierung</h4>
            <p>„Das ist gar nicht teuer, wenn Sie mal nachrechnen..." <br>— Wirkt herablassend und ignoriert die Perspektive des Kunden vollständig.</p>
          </div>
        </div>
      </div>
    </div>
    <div class="fw-step">
      <div class="fw-num">E</div>
      <div class="fw-body">
        <h4>Ergründen & Isolieren – Erst verstehen, dann handeln</h4>
        <p>Frage nach den Details, um den Einwand präzise zu verstehen. Nutze die Isolationsfrage aus Modul 1. Erst wenn du sicher bist, dass du den echten, einzigen Einwand kennst, macht es Sinn, ihn zu behandeln. Ein häufiger Fehler: Der Vertriebler löst den Budget-Einwand – und merkt dann, dass die IT-Abteilung sowieso nie zugestimmt hätte.</p>
        <div class="skript-box" style="margin-top:.75rem">
          <div class="sk-label">💬 Ergründungs-Fragen</div>
          <div class="sk-text">„Darf ich kurz nachfragen – wenn Sie von ‚zu teuer' sprechen: Beziehen Sie sich dabei auf das Budget insgesamt, oder auf den Vergleich mit einem anderen Anbieter?"<br><br>„Was genau meinen Sie, wenn Sie sagen, dass Sie das intern prüfen müssen – an wen müsste das noch?"<br><br>„Angenommen, das wäre gelöst – würde dann noch etwas gegen das Projekt sprechen?"</div>
        </div>
      </div>
    </div>
    <div class="fw-step">
      <div class="fw-num">V</div>
      <div class="fw-body">
        <h4>Verändern & Lösen – Die Brücke zum Abschluss</h4>
        <p>Jetzt – und erst jetzt – behandelst du den Einwand. Nicht mit einer langen Verteidigung, sondern mit einer neuen Perspektive. Das Ziel ist nicht, den Kunden zu überwältigen, sondern ihm eine neue Sichtweise zu öffnen, die er selbst für logisch hält. Und: Verbinde die Lösung immer mit einem konkreten Abschluss-Trigger.</p>
        <p style="font-size:12px;color:#6B7280;margin-top:.4rem">Falsch: Einwand lösen → Pause → Hoffen. Richtig: Einwand lösen → direkt Bridge zum nächsten Schritt bauen.</p>
      </div>
    </div>
  </div>

  <h3>LAEV in der Praxis – komplettes Gesprächsbeispiel</h3>
  <div class="skript-box">
    <div class="sk-label">💬 Vollständiges Beispiel-Skript: Einwand „Zu teuer"</div>
    <div class="sk-text">Kunde: „Ihr Angebot ist deutlich teurer als das der Konkurrenz."

L – (2 Sekunden Pause, dann ruhig): „Ich höre Sie."

A – Anerkennen: „Ich kann das vollkommen nachvollziehen. Bei einem Investment in dieser Größenordnung ist es absolut richtig, jeden Euro zu hinterfragen. Das zeigt mir, dass Sie kein Projekt mal eben durchwinken."

E – Ergründen: „Darf ich kurz fragen – wenn Sie von teurer sprechen: Vergleichen Sie uns mit einem konkreten Mitbewerberangebot, oder geht es um das Budget insgesamt? Und: Angenommen, der Preis wäre für Sie kein Thema – gäbe es dann noch andere Punkte, die Sie zögern lassen würden?"

(Kunde: „Nein, eigentlich nur der Preis.")

V – Verändern & Lösen: „Gut, dann lassen Sie uns das kurz gemeinsam durchleuchten. Wenn wir uns den Betrieb über 5 Jahre anschauen, kostet Sie unser System trotz der höheren Anschaffung insgesamt ca. 38.000 € weniger als das Alternativangebot – durch geringere Energiekosten, niedrigere Wartungsaufwände und weniger Ausfallzeiten. Ich kann Ihnen das in einem kurzen TCO-Sheet transparent aufzeigen. Sollen wir dafür die nächste Woche einen 30-Minuten-Termin ansetzen?"</div>
  </div>

  <h3>Häufige Fehler beim LAEV-Framework</h3>
  <div class="tbl-wrap"><table>
    <thead><tr><th>Fehler</th><th>Warum er passiert</th><th>Konsequenz</th></tr></thead>
    <tbody>
      <tr><td>Sofort zur Lösung springen (kein L-A)</td><td>Nervosität, Angst vor Stille</td><td>Kunde fühlt sich nicht gehört, erhöhte Abwehr</td></tr>
      <tr><td>Validieren ohne E (Isolation überspringen)</td><td>Ungeduld, „Budget ist klar genug"</td><td>Man behandelt Vorwand, echter Einwand bleibt</td></tr>
      <tr><td>Einwand lösen ohne Abschluss-Trigger</td><td>Angst vor dem Abschluss</td><td>Guter Einwand-Konter, aber kein Vorwärtsbewegen</td></tr>
      <tr><td>Zu viel Reden beim Validieren</td><td>Will dem Kunden zeigen, dass man versteht</td><td>Wirkt unecht und einstudiert</td></tr>
    </tbody>
  </table></div>

  <div class="aufgabe-box">
    <h4>📝 Praxis-Übung (5 Min.)</h4>
    <ol>
      <li>Nimm den häufigsten Einwand, den du regelmäßig hörst. Schreibe das vollständige LAEV-Skript dafür auf.</li>
      <li>Lies es laut vor. Klingt das L und A natürlich? Falls nein – formuliere es um, bis es wie ein echtes Gespräch klingt.</li>
      <li>Bitte einen Kollegen, den Einwand zu spielen. Führe das Gespräch durch. Videographiere dich selbst wenn möglich.</li>
    </ol>
  </div>

  <div class="mquiz">
    <h4>🎯 Quick-Check</h4>
    <div class="qtext">In welcher Reihenfolge läuft das LAEV-Framework ab?</div>
    <button class="mopt" onclick="mqPick(this,'m1q1','a')"><span class="dot"></span>Lösen → Anerkennen → Ergründen → Lauschen</button>
    <button class="mopt" onclick="mqPick(this,'m1q1','b')"><span class="dot"></span>Lauschen → Anerkennen → Ergründen & Isolieren → Verändern & Lösen</button>
    <button class="mopt" onclick="mqPick(this,'m1q1','c')"><span class="dot"></span>Anerkennen → Lauschen → Lösen → Ergründen</button>
    <div class="mfb ok" id="mq-m1q1-ok">✓ Richtig! Erst lauschen und den Kunden ausreden lassen, dann validieren, dann isolieren – und erst zuletzt lösen. Die Reihenfolge ist nicht verhandelbar.</div>
    <div class="mfb err" id="mq-m1q1-err">✗ Die Reihenfolge ist: Lauschen → Anerkennen → Ergründen & Isolieren → Verändern & Lösen. Wer zuerst löst, ohne zu isolieren, behandelt fast immer den falschen Einwand.</div>
  </div>
  <div class="nav-btns">
    <button class="btn" onclick="showMod(0)">← Zurück</button>
    <button class="btn btn-primary" onclick="nextMod(1)">Weiter: Die 3 Top-Einwände →</button>
  </div>
</div>
</div>

<!-- ══════════════════ MODULE 2: DIE 3 TOP-EINWÄNDE ══ -->
<div class="module" id="m2">
<div class="card">
  <div class="mod-title"><span class="mico">⚔️</span>Die 3 härtesten B2B-Einwände – Tiefen-Analyse &amp; Skripte</div>
  <p>Diese drei Einwände begegnest du täglich. Hier bekommst du nicht nur das Skript – du verstehst auch die Psychologie dahinter, warum der Einwand wirklich kommt und warum diese Antwort funktioniert.</p>

  <h3>Einwand 1: „Sie sind zu teuer! Der Mitbewerber ist 20% günstiger."</h3>
  <p><strong>Warum dieser Einwand kommt:</strong> Der Kunde hat zwei Zahlen auf einem Blatt Papier. Er sieht nicht den Unterschied in Qualität, Effizienz, Ausfallsicherheit oder Lebensdauer – er sieht nur eine höhere Zahl. Das ist kein Intelligenz-Problem, sondern ein Rahmenproblem: Der falsche Vergleichsrahmen wurde gesetzt (Anschaffungspreis statt Total Cost of Ownership).</p>
  <p><strong>Psychologische Basis:</strong> Menschen neigen dazu, leicht messbare Größen überzubewerten (Anschaffungspreis = sofort messbar) und schwer messbare zu ignorieren (Betriebskosten über 5 Jahre = abstrakt). Deine Aufgabe: Den Rahmen wechseln.</p>

  <div class="skript-box">
    <div class="sk-label">💬 Schritt 1: Die ROI-Umdrehungs-Frage</div>
    <div class="sk-text">„Herr [Name], ich verstehe vollkommen. Wenn man zwei Angebote nebeneinanderlegt und auf die Gesamtsumme schaut, wirkt unser Investment im ersten Moment höher.

Darf ich Ihnen ganz offen eine Frage stellen: Suchen Sie nach der Anlage, die in der Anschaffung die billigste ist – oder nach der, die über die nächsten 5 Jahre im Betrieb die niedrigsten Gesamtkosten und die höchste Ausfallsicherheit garantiert?"</div>
    <div class="sk-note">→ Jetzt schweigen. Der Kunde antwortet fast immer mit „Natürlich die günstigeren Betriebskosten." Damit hat er selbst zugegeben, dass der Anschaffungspreis das falsche Kriterium war.</div>
  </div>

  <div class="skript-box">
    <div class="sk-label">💬 Schritt 2: Die TCO-Rechnung aufmachen</div>
    <div class="sk-text">„Genau da liegt der Unterschied. Wenn wir uns anschauen, was die 20% Differenz in der Anschaffung wirklich bedeutet:

Die geringere Effizienz des Mitbewerbers kostet Sie jährlich ca. 18.000 € mehr an Energie und Wartung. Das bedeutet: Schon nach 14 Monaten zahlen Sie bei der vermeintlich günstigeren Lösung drauf – nicht wir.

Über 5 Jahre sprechen wir von einem TCO-Vorteil von ca. 72.000 € auf unserer Seite. Das ist die eigentliche Entscheidungsgrundlage.

Wollen wir das so aufsetzen, dass die Anlage sich für Sie ab Monat 1 amortisiert – oder möchten Sie das Risiko der laufenden Mehrkosten eingehen?"</div>
  </div>

  <h3>Warum du niemals sofort Rabatt gibst</h3>
  <p>Jeder sofortige Rabatt sendet zwei fatale Signale gleichzeitig: Erstens, dass du vorher gelogen und zu teuer angeboten hast. Zweitens, dass weitere Zugeständnisse möglich sind. Du öffnest eine Tür, die du nie wieder schließen kannst.</p>
  <div class="hl-amber"><strong>Die 24-Stunden-Regel:</strong> Wenn der Preisdruck zu stark wird und du überlegen musst ob ein Zugeständnis möglich ist, sage nie direkt Nein und nie direkt Ja. Antworte: „Ich prüfe intern, was ich für Sie tun kann – ich melde mich bis morgen Mittag." Das gibt dir Zeit, eine durchdachte Gegenleistungs-Forderung vorzubereiten.</div>

  <h3>Einwand 2: „Wir haben bereits einen festen Partner und sind zufrieden."</h3>
  <p><strong>Warum dieser Einwand kommt:</strong> „Never change a running system" ist ein tief verwurzeltes Prinzip in der Unternehmensführung. Der Aufwand eines Lieferantenwechsels (neue Verträge, neue Schulungen, neues Risiko) wird emotional als sehr hoch bewertet – selbst wenn die aktuelle Lösung objektiv schlechter ist.</p>
  <p><strong>Dein Fehler wäre:</strong> Sofort den Wettbewerber schlechtzureden. Das macht dich unglaubwürdig, weil du den Partner des Kunden angreifst – und damit indirekt die Entscheidung des Kunden, diesen Partner gewählt zu haben.</p>

  <div class="skript-box">
    <div class="sk-label">💬 Elite-Skript: Die Benchmark-Taktik</div>
    <div class="sk-text">„Es freut mich wirklich zu hören, dass Sie einen verlässlichen Partner haben – das zeigt mir, wie wichtig Ihnen Kontinuität und Qualität in diesem Bereich sind. Und ich bin heute auch nicht hier, um diesen Partner schlechtzureden.

Ich stelle Ihnen lediglich eine strategische Frage: Selbst wenn Sie aktuell zufrieden sind – macht es als Entscheider nicht Sinn, sich alle 18 bis 24 Monate einen Zweit-Benchmark einzuholen? Einfach um sicherzustellen, dass Sie technisch noch auf dem neuesten Stand sind – und dass Ihr aktueller Partner Ihnen wirklich die besten Konditionen bietet?

Mein Vorschlag ist konkret: Lassen Sie uns für das nächste Teilprojekt – nur dieses eine – einen unverbindlichen Proof-of-Concept machen. Wenn wir besser sind, haben Sie eine valide Alternative. Wenn wir nicht besser sind, haben Sie die Gewissheit, dass Ihr aktueller Partner einen Top-Job macht. Was spricht aus Ihrer Sicht dagegen, sich diese Absicherung zu holen?"</div>
  </div>

  <div class="hl-blue"><strong>Die Psychologie dahinter:</strong> Du forderst keinen Wechsel. Du bietest Absicherung und Bestätigung an. Jeder rationale Entscheider, der das hört, kann nicht ablehnen ohne zuzugeben, dass er bewusst Alternativen ignoriert. Du senkst die wahrgenommene Risikobarriere auf null.</div>

  <h3>Einwand 3: „Das hat aktuell keine Priorität – wir machen das nächstes Jahr."</h3>
  <p><strong>Warum dieser Einwand kommt:</strong> Aufschieberitis entsteht fast immer aus einem dieser drei Gründe: 1) Der Implementierungsaufwand erscheint zu hoch, 2) es fehlt ein interner Champion der das Projekt vorantreibt, oder 3) der Schmerz des Status quo wurde noch nicht konkret genug gemacht. „Nächstes Jahr" ist die bequemste Art, nein zu sagen ohne nein zu sagen.</p>

  <div class="skript-box">
    <div class="sk-label">💬 Elite-Skript: Die Cost-of-Inaction-Methode</div>
    <div class="sk-text">„Ich verstehe, dass Ihr Tisch aktuell voll ist – das hören wir in der Branche gerade häufig. 'Nächstes Jahr' klingt im ersten Moment sicherer. Lassen Sie uns aber kurz gemeinsam in die Realität schauen, bevor wir das so stehen lassen:

Jedes Monat, das Sie diese Anlage nicht im Betrieb haben, verlieren Sie durch die alten Systeme exakt [Betrag, z. B. 4.200 €] an Marge – direkt vom Gewinn. Das sind nicht zukünftige Gewinne die ausbleiben, sondern reales Geld das heute verbrannt wird.

Bis zum nächsten Jahr sprechen wir von ca. [Betrag × 12, z. B. 50.400 €] verbranntem Kapital, das unwiderruflich verloren ist.

Wenn wir das Projekt jetzt starten, übernehmen wir die komplette Projektleitung. Ihr Team ist mit weniger als 2 Stunden pro Woche involviert. Im nächsten Jahr ernten Sie bereits die Früchte.

Die Frage ist also nicht: Können wir uns das leisten? Die Frage ist: Können wir es uns leisten, es ein weiteres Jahr aufzuschieben?"</div>
  </div>

  <h3>So berechnest du die Cost of Inaction für jeden Kunden individuell</h3>
  <div class="tbl-wrap"><table>
    <thead><tr><th>Kostentreiber</th><th>Typische Größenordnung</th><th>Beispielberechnung</th></tr></thead>
    <tbody>
      <tr><td>Energiemehrkosten alte Anlage</td><td>800–3.500 €/Monat</td><td>Anlage mit SCOP 2,5 vs. Realm SCOP 4,5 → ~1.200 €/Monat</td></tr>
      <tr><td>Wartungskosten alte Anlage</td><td>400–1.200 €/Monat</td><td>Alter Gaskessel mit häufigen Störungen → 600 €/Monat</td></tr>
      <tr><td>Ausfallrisiko</td><td>500–5.000 €/Monat (kalkulatorisch)</td><td>Kritische Anlage mit 2% Ausfallrisiko und 40 €/h Produktionsausfall</td></tr>
      <tr><td>Verpasste Förderung</td><td>Einmalig 10.000–21.000 €</td><td>BAFA-Förderung 70% auf max. 30.000 € = bis 21.000 €</td></tr>
      <tr><td><strong>Summe pro Monat</strong></td><td><strong>2.000–10.000 €</strong></td><td><strong>Konkrete Zahl ins Gespräch einbauen</strong></td></tr>
    </tbody>
  </table></div>

  <div class="aufgabe-box">
    <h4>📝 Praxis-Übung (7 Min.)</h4>
    <ol>
      <li>Wähle deinen aktuell stockendsten Deal. Welcher der 3 Einwände ist der wahrscheinlichste?</li>
      <li>Schreibe das Skript für genau diesen Deal mit den realen Zahlen dieses Kunden aus.</li>
      <li>Berechne die Cost of Inaction konkret: Was kostet ihn jeder weitere Monat Verzögerung in Euro?</li>
      <li>Sprich das vollständige Skript dreimal laut aus. Es muss ruhig, sachlich und partnerschaftlich klingen – nie aggressiv.</li>
    </ol>
  </div>

  <div class="nav-btns">
    <button class="btn" onclick="showMod(1)">← Zurück</button>
    <button class="btn btn-primary" onclick="nextMod(2)">Weiter: Closing-Frameworks →</button>
  </div>
</div>
</div>

<!-- ══════════════════ MODULE 3: CLOSING ══ -->
<div class="module" id="m3">
<div class="card">
  <div class="mod-title"><span class="mico">🎯</span>B2B Closing-Frameworks – Verbindlichkeits-Architektur</div>
  <p>Im B2B-Vertrieb gibt es den einen „magischen Closing-Satz" schlichtweg nicht. Ein B2B-CFO oder Geschäftsführer wird durch billige Drücker-Methoden nicht zur Unterschrift gezwungen – er verliert nur das Vertrauen in dich und kauft woanders.</p>
  <div class="highlight"><strong>Goldene Regel:</strong> Abschluss ist ein Prozess, kein einzelnes Event. Ein B2B-Entscheider unterschreibt, wenn das Risiko des Nicht-Handelns größer ist als das Risiko der Investition. Du baust dieses Ungleichgewicht durch <em>Micro-Commitments</em> auf, die sich durch das gesamte Gespräch ziehen.</div>

  <h3>Was Micro-Commitments sind – und warum sie entscheidend sind</h3>
  <p>Ein Micro-Commitment ist jede kleine Zustimmung des Kunden im Verlauf des Gesprächs. „Stimmt das mit dem Zeitplan?" – Ja. „Wäre das technisch umsetzbar?" – Ja. „Macht der ROI für Sie Sinn?" – Ja. Jedes dieser Jas baut eine Verbindlichkeit auf. Am Ende des Gesprächs ist der Abschluss keine große neue Entscheidung mehr – er ist die logische Konsequenz von 8–12 kleinen Zustimmungen.</p>

  <h3>Framework 1: Der Implementation Blueprint</h3>
  <p><strong>Wann einsetzen:</strong> Wenn der Kunde grundsätzlich zustimmt, aber zögert und die Entscheidung hinausschiebt. Das Blueprint-Closing lenkt seinen Blick weg vom Geld und hin zur konkreten, positiven Zukunft. Er denkt nicht mehr darüber nach ob er kauft – er denkt über die Implementierung nach.</p>
  <div class="skript-box">
    <div class="sk-label">💬 Skript: Implementation Blueprint Closing</div>
    <div class="sk-text">„Herr [Name], nachdem wir alle technischen Details und den ROI von [Betrag] € gemeinsam geklärt haben, lassen Sie uns kurz auf den Kalender schauen – damit das Projekt bei Ihnen intern reibungslos anläuft.

Wenn wir die vertraglichen Details diese Woche abschließen, können unsere Ingenieure in KW [X] für das Kick-off-Meeting bei Ihnen vor Ort sein. Die Lieferung und Montage erfolgt dann planmäßig in KW [Y], sodass die Anlage pünktlich zum Start des neuen Quartals in Betrieb ist.

Ihr Team muss dafür in den ersten zwei Wochen ca. 3–4 Stunden einplanen – danach läuft alles automatisch. Spricht aus Ihrer Sicht etwas gegen diesen Zeitplan, oder sollen wir das Projekt für KW [X] so einloggen?"</div>
    <div class="sk-note">→ Du fragst nicht ob er kauft. Du fragst ob der Zeitplan passt. Das ist der Unterschied.</div>
  </div>

  <h3>Framework 2: Cost of Inaction Closing</h3>
  <p><strong>Warum es funktioniert:</strong> Verlust-Aversion ist eines der stärksten psychologischen Prinzipien (Kahneman, Nobelpreis 2002). Menschen reagieren ca. 2–2,5× stärker auf den Verlust von bestehendem Geld als auf die Aussicht auf neues Geld. „Sie verlieren 6.500 € pro Monat" ist deutlich stärker als „Sie könnten 6.500 € pro Monat gewinnen".</p>
  <div class="skript-box">
    <div class="sk-label">💬 Skript: Cost of Inaction Closing</div>
    <div class="sk-text">„Frau [Name], ich verstehe vollkommen, dass eine Investition in dieser Größenordnung eine fundierte Entscheidung braucht. Lassen Sie uns das kurz betriebswirtschaftlich validieren – ich zeige Ihnen, was die Bedenkzeit wirklich kostet:

Wir haben vorhin gemeinsam errechnet, dass Sie durch die Ineffizienz Ihrer aktuellen Anlage jeden Monat exakt 6.500 € netto verlieren. Das ist kein theoretischer Wert – das sind echte Euros die täglich vom Gewinn abgehen.

Wenn wir die Entscheidung jetzt um vier Wochen vertagen, kostet Sie dieses eine 'Bedenkzeit-Monat' 6.500 €, die unwiderruflich verloren sind. Diese Kosten entstehen unabhängig davon, ob Sie kaufen oder nicht.

Mein Vorschlag: Lassen Sie uns das Projekt heute freigeben. Damit stoppen wir diesen Verlust ab Tag 1 der Implementierung. Kleines Detail zur Abwicklung: Sollen wir den Vertrag auf die Holding oder direkt auf Ihre operative Gesellschaft ausstellen?"</div>
    <div class="sk-note">→ Einsatz: Bei Kunden die verschieben oder „noch eine Nacht drüber schlafen" wollen. Die letzte Frage leitet direkt zur Unterschrift über.</div>
  </div>

  <h3>Framework 3: Alternative / Conditional Closing</h3>
  <p><strong>Die Psychologie:</strong> Wenn ein Kunde das Gefühl hat, er wird zur Unterschrift gedrängt, aktiviert das Reaktanz – den psychologischen Widerstand gegen wahrgenommenen Kontrollverlust. Das Alternative Closing gibt dem Kunden das Gefühl, die Kontrolle zu haben – über den Prozess, nicht über das ob. Der Unterschied ist entscheidend.</p>
  <div class="skript-box">
    <div class="sk-label">💬 Skript: Alternative / Conditional Closing</div>
    <div class="sk-text">„Herr [Name], von unserer Seite steht dem Projekt nichts im Wege – wir können jederzeit starten. Um die internen Prozesse bei uns anzustoßen, gibt es zwei Wege: Entweder senden wir Ihnen den Vertragsentwurf direkt als digitalen Signatur-Link über DocuSign zu – das dauert auf beiden Seiten keine 5 Minuten. Oder wir stimmen den Entwurf vorab in einer kurzen Schleife mit Ihrer Rechts- oder Finanzabteilung ab, wenn das intern sauberer ist.

Welcher dieser beiden Wege ist für Ihre internen Abläufe der effizientere?"</div>
    <div class="sk-note">→ Du fragst nicht: „Wollen Sie kaufen?" Du fragst: „Wie wollen Sie kaufen?" Das ist der entscheidende Unterschied zwischen Drücker und Profi.</div>
  </div>

  <h3>Wann welches Framework einsetzen – Schnellübersicht</h3>
  <div class="tbl-wrap"><table>
    <thead><tr><th>Situation</th><th>Richtiges Framework</th><th>Kernbotschaft</th></tr></thead>
    <tbody>
      <tr><td>Kunde sagt „Ja, aber ich muss noch..." und zögert</td><td>Implementation Blueprint</td><td>Zeitplan konkretisieren, Zukunft visualisieren</td></tr>
      <tr><td>Kunde sagt „Nächstes Jahr" oder „Nochmal drüber schlafen"</td><td>Cost of Inaction</td><td>Kosten des Wartens konkret in Euro benennen</td></tr>
      <tr><td>Gespräch ist positiv, Entscheidung nahe, Process unklar</td><td>Alternative Closing</td><td>Kontrolle über den Prozess geben, nicht über das ob</td></tr>
      <tr><td>Einwände wurden alle ausgeräumt, Stille entsteht</td><td>Implementation Blueprint + Conditional</td><td>Kombination: Zeitplan besprechen UND Prozessweg klären</td></tr>
    </tbody>
  </table></div>

  <div class="aufgabe-box">
    <h4>📝 Praxis-Übung (7 Min.)</h4>
    <ol>
      <li>Nimm deinen aktuell wichtigsten Deal. In welcher Situation befindet er sich gerade – und welches der drei Frameworks passt?</li>
      <li>Schreibe das passende Closing-Skript mit den konkreten Zahlen dieses Deals.</li>
      <li>Formuliere 3 Micro-Commitment-Fragen für das nächste Gespräch – Fragen, bei denen der Kunde nur Ja sagen kann.</li>
    </ol>
  </div>

  <div class="nav-btns">
    <button class="btn" onclick="showMod(2)">← Zurück</button>
    <button class="btn btn-primary" onclick="nextMod(3)">Weiter: Anti-Ghosting →</button>
  </div>
</div>
</div>

<!-- ══════════════════ MODULE 4: ANTI-GHOSTING ══ -->
<div class="module" id="m4">
<div class="card">
  <div class="mod-title"><span class="mico">👻</span>Das Anti-Ghosting-Protokoll – Deals aus dem schwarzen Loch retten</div>
  <p>Ghosting ist das teuerste Problem im B2B-Vertrieb. Du investierst Stunden in Qualifizierung, Präsentation und Angebotserstellung – und dann: Stille. Das Angebot ist raus. Der Kunde reagiert nicht mehr. Du rufst an, er geht nicht ran. Du schreibst, er antwortet nicht.</p>
  <p>Das ist kein Zufall. Das passiert fast immer aus einem dieser Gründe: Der Entscheider ist intern unter Druck geraten, ein interner Wettbewerber blockiert das Projekt, oder das Angebot wurde nie wirklich besprochen – es liegt irgendwo in einem E-Mail-Ordner.</p>
  <div class="hl-red"><strong>Die einzige Lösung: Prävention.</strong> Du kannst Ghosting nicht reparieren – du kannst es nur verhindern. Das tust du mit einem einzigen Grundsatz: Kein Angebot verlässt dein Büro, ohne dass gleichzeitig ein fester Besprechungstermin im Kalender des Kunden verankert ist.</div>

  <h3>Warum Ghosting so häufig passiert – die 5 wahren Ursachen</h3>
  <div class="tbl-wrap"><table>
    <thead><tr><th>Ursache</th><th>Was dahintersteckt</th><th>Prävention</th></tr></thead>
    <tbody>
      <tr><td>Kein Folgetermin vereinbart</td><td>Das Angebot landet im E-Mail-Ordner und wird begraben</td><td>No-Offer-Without-Date Regel eisern einhalten</td></tr>
      <tr><td>Interner Widerstand beim Kunden</td><td>Jemand intern blockiert das Projekt (IT, Einkauf, CFO)</td><td>Im Gespräch Champion identifizieren und stärken</td></tr>
      <tr><td>Neues internes Projekt verdrängt</td><td>Dein Deal hat Priorität verloren durch externe Ereignisse</td><td>Cost of Inaction im Gespräch stark verankern</td></tr>
      <tr><td>Entscheider hat intern keine Kompetenz</td><td>Er braucht Genehmigung, traut sich aber nicht zu sagen</td><td>Ergründen: „Wen müsste das Projekt noch überzeugen?"</td></tr>
      <tr><td>Konkurrenz hat nachgefasst</td><td>Ein Wettbewerber war hartnäckiger oder günstiger</td><td>Schnelleres Follow-up, Break-up-E-Mail früher einsetzen</td></tr>
    </tbody>
  </table></div>

  <h3>Das „No-Offer-Without-Date"-Protokoll</h3>
  <p>Diese Regel ist nicht verhandelbar. Sie gilt ausnahmslos. Jedes Angebot das du ohne Folgetermin versendest, hat eine Ghosting-Wahrscheinlichkeit von über 60%.</p>
  <div class="skript-box">
    <div class="sk-label">💬 Skript: Folgetermin sichern – Version A (direkt)</div>
    <div class="sk-text">„Herr [Name], ich erstelle Ihnen sehr gerne das maßgeschneiderte Angebot inklusive der besprochenen Staffelung. Da es sich hierbei um ein investitionsrelevantes Dokument handelt, ist mir eines wichtig: Ich möchte Sie nicht mit 15–20 Seiten Zahlenmaterial allein lassen.

Lassen Sie uns direkt jetzt unsere Kalender öffnen und einen kurzen, 15-minütigen Termin vereinbaren – ich sage Ihnen nächsten Dienstag 10:00 Uhr oder Donnerstag 14:00 Uhr. Wir gehen das Angebot gemeinsam durch, ich beantworte alle Fragen und wir können sofort Anpassungen vornehmen. Welcher der beiden Termine passt Ihnen besser?"</div>
    <div class="sk-note">→ Du gibst zwei konkrete Alternativen – keine offene Frage. Das erzeugt eine binäre Entscheidung statt einer Ausflucht.</div>
  </div>

  <div class="skript-box">
    <div class="sk-label">💬 Skript: Wenn der Kunde „einfach so" schicken will</div>
    <div class="sk-text">„Das mache ich gerne für Sie. Ich habe aber aus 12 Jahren Praxis gelernt: Wenn ein Angebot in dieser Komplexität ohne Durchsprache rausgeht, entstehen fast immer Rückfragen – und die lösen sich per E-Mail über Tage und Wochen, nicht Stunden.

Mein Qualitätsanspruch beginnt schon beim Angebotsprozess. Die 15 Minuten, die wir investieren, sparen Ihnen das Dreifache an E-Mail-Pingpong. Welcher Tag der nächsten Woche passt für Sie besser – Dienstag oder Mittwoch?"</div>
  </div>

  <h3>Das Nachfass-Protokoll – strukturiertes Follow-up nach dem Angebot</h3>
  <p>Wenn der Termin vereinbart ist und nach der Durchsprache keine Entscheidung kommt, greift das strukturierte Follow-up:</p>
  <div class="steps">
    <div class="step"><div class="step-num">T+1</div><div class="step-body"><h4>Tag nach der Angebotsbesprechung</h4><p>Kurze Zusammenfassungs-E-Mail: „Schön, dass wir das durchgehen konnten. Hier nochmal die wichtigsten Punkte. Wann können wir mit Ihrer Entscheidung rechnen?"</p></div></div>
    <div class="step"><div class="step-num">T+5</div><div class="step-body"><h4>5 Tage nach Angebot</h4><p>Telefonat: „Haben Sie Fragen zum Angebot? Ich wollte sicherstellen, dass alle Punkte klar sind." Nicht fragen ob er sich entschieden hat – sondern ob er Fragen hat.</p></div></div>
    <div class="step"><div class="step-num">T+10</div><div class="step-body"><h4>10 Tage – leichter Urgency-Trigger</h4><p>E-Mail mit neuem Inhalt: „Wir haben gerade unser letztes Montagefenster in KW [X] vergeben – für Sie würde ich aber noch prüfen ob etwas freigemacht werden kann. Gibt es von Ihrer Seite einen Update?"</p></div></div>
    <div class="step"><div class="step-num">T+14</div><div class="step-body"><h4>14 Tage – Break-up-E-Mail</h4><p>Wenn keine Reaktion kommt: Break-up-E-Mail versenden. Keine weiteren Versuche davor.</p></div></div>
  </div>

  <h3>Die Break-up-E-Mail – das stärkste Instrument gegen stagnierende Deals</h3>
  <div class="email-box">
    <div class="email-header">✉ Die Break-up-E-Mail – Word-for-Word</div>
    <div class="email-subject">Betreff: Unser Projekt [Projektname] / Schließung der Akte</div>
    <div class="email-body">Sehr geehrte/r Frau/Herr [Name],

da ich in den letzten zwei Wochen nichts mehr von Ihnen gehört habe, gehe ich davon aus, dass sich Ihre Prioritäten intern verschoben haben oder das Projekt [Thema] aktuell keine Relevanz mehr für Sie hat.

Da wir unsere Kapazitäten für die Projektierung und Montage im kommenden Quartal exakt planen müssen, werde ich den Vorgang bei uns vorerst auf „inaktiv" setzen und die reservierten Ressourcen wieder freigeben.

Sollte das Thema zu einem späteren Zeitpunkt wieder für Sie aktuell werden, können wir die Gespräche gerne neu aufrollen – dann aber unter Umständen zu anderen Konditionen und Lieferterminen.

Ich wünsche Ihnen für Ihre anstehenden Projekte alles Gute.

Mit freundlichen Grüßen
[Dein Name]</div>
  </div>

  <div class="hl-amber"><strong>Was in der Praxis passiert:</strong> Ein Entscheider, der das Projekt wirklich will aber im Stress war, antwortet innerhalb von 4 Stunden: „Bitte nicht schließen – ich hatte [Grund]. Können wir nächste Woche telefonieren?" Das ist ein Gewinn. Wenn er nicht antwortet, war der Deal ohnehin tot – und du hast wertvolle mentale Energie für echte Chancen frei.</div>

  <h3>Pipeline-Hygiene: Wann ein Deal als tot gilt</h3>
  <div class="tbl-wrap"><table>
    <thead><tr><th>Signal</th><th>Bedeutung</th><th>Maßnahme</th></tr></thead>
    <tbody>
      <tr><td>Keine Reaktion auf 3 Versuche in 2 Wochen</td><td>Deal ist inaktiv</td><td>Break-up-E-Mail, dann auf inaktiv setzen</td></tr>
      <tr><td>Immer wieder „nächste Woche"</td><td>Kein interner Champion vorhanden</td><td>Champion-Frage stellen: „Wer intern könnte das Projekt vorantreiben?"</td></tr>
      <tr><td>Entscheider nicht mehr erreichbar</td><td>Positionswechsel oder interner Konflikt</td><td>Neuen Kontakt im Unternehmen suchen</td></tr>
      <tr><td>Deal in Pipeline seit >90 Tagen ohne Bewegung</td><td>Pipeline-Illusion – blockiert mentale Energie</td><td>Ehrliche Re-Qualifizierung oder Break-up</td></tr>
    </tbody>
  </table></div>

  <div class="aufgabe-box">
    <h4>📝 Sofort-Aufgabe (5 Min.)</h4>
    <ol>
      <li>Öffne dein CRM oder deine Angebotsliste. Wie viele offene Angebote sind älter als 14 Tage ohne konkreten Folgetermin?</li>
      <li>Für jeden dieser Deals: Heute noch die Break-up-E-Mail versenden – oder sofort einen Termin vereinbaren.</li>
      <li>Lege dir eine Erinnerung ein: Kein Angebot ohne Datum. Immer. Ausnahmslos.</li>
    </ol>
  </div>

  <div class="nav-btns">
    <button class="btn" onclick="showMod(3)">← Zurück</button>
    <button class="btn btn-primary" onclick="nextMod(4)">Weiter: Key Account &amp; Upsell →</button>
  </div>
</div>
</div>

<!-- ══════════════════ MODULE 5: KEY ACCOUNT ══ -->
<div class="module" id="m5">
<div class="card">
  <div class="mod-title"><span class="mico">📈</span>Key Account Management &amp; Strategisches Up-Selling</div>
  <p>Viele Vertriebler begehen nach dem Closing den fatalen Fehler, den Kunden an den Service zu übergeben und sich wieder der Neukundenakquise zu widmen. Sie glauben, der Deal ist gemacht. In Wirklichkeit hat er gerade erst begonnen.</p>
  <div class="highlight"><strong>Goldene Regel: Die echte Akquise beginnt nach dem Kauf.</strong> Die Wahrscheinlichkeit, an einen zufriedenen B2B-Bestandskunden zu verkaufen, liegt bei 60–70%. Bei einem kalten Lead: 5–20%. Das bedeutet: Dein Bestandskundenbuch ist deine profitabelste Pipeline – sie wird nur von den wenigsten aktiv bearbeitet.</div>

  <h3>Die 3 Entwicklungsstufen einer Kundenbeziehung</h3>
  <p>Jede Kundenbeziehung durchläuft idealerweise drei Stufen. Dein Ziel ist Stufe 3 – und der Weg dorthin ist ein aktiver Prozess, kein Zufall.</p>
  <div class="framework-steps">
    <div class="fw-step">
      <div class="fw-num">1</div>
      <div class="fw-body">
        <h4>Stufe 1: Transaktions-Lieferant</h4>
        <p>Du wirst ausschließlich über Preis und Lieferzeit definiert. Der Kunde fragt bei jedem Projekt neu an – und vergleicht immer mit Wettbewerbern. Austauschbarkeit: extrem hoch. Auf dieser Stufe verliert man Kunden an den billigsten Anbieter, sobald dieser existiert.</p>
        <p style="font-size:12px;color:#6B7280;margin-top:.3rem">Erkennungszeichen: Kein persönlicher Kontakt zum Entscheider, immer Einkaufsabteilung als Ansprechpartner, Angebote werden systematisch verglichen.</p>
      </div>
    </div>
    <div class="fw-step">
      <div class="fw-num">2</div>
      <div class="fw-body">
        <h4>Stufe 2: Bevorzugter Anbieter</h4>
        <p>Du hast bewiesen, dass Qualität und Service stimmen. Man fragt dich bei neuen Projekten automatisch als ersten an. Du wirst bevorzugt behandelt – aber trotzdem noch mit anderen verglichen. Ein guter Ausgangspunkt für Up-Selling, aber noch keine stabile Partnerschaft.</p>
        <p style="font-size:12px;color:#6B7280;margin-top:.3rem">Erkennungszeichen: Direktanfragen ohne Ausschreibung, aber noch kein Einblick in strategische Planungen.</p>
      </div>
    </div>
    <div class="fw-step">
      <div class="fw-num">3</div>
      <div class="fw-body">
        <h4>Stufe 3: Strategischer Partner</h4>
        <p>Du wirst vor der Budgetplanung an den Tisch geholt. Der Kunde teilt seine 3- bis 5-Jahres-Strategie mit dir, damit du deine Lösungen daran ausrichtest. Austauschbarkeit: nahezu null. Du bist kein Lieferant mehr – du bist Teil des Unternehmens aus der Außenperspektive.</p>
        <p style="font-size:12px;color:#6B7280;margin-top:.3rem">Erkennungszeichen: Einladungen zu strategischen Meetings, Einblick in Wachstumspläne, Empfehlung an Tochtergesellschaften.</p>
      </div>
    </div>
  </div>

  <h3>Wie du von Stufe 1 auf Stufe 3 kommst – die konkreten Hebel</h3>
  <div class="tbl-wrap"><table>
    <thead><tr><th>Von Stufe</th><th>Auf Stufe</th><th>Was du tust</th></tr></thead>
    <tbody>
      <tr><td>1 → 2</td><td>Bevorzugter Anbieter</td><td>Liefere das Versprochene, übertriff Erwartungen beim ersten Projekt, baue persönlichen Kontakt zum Entscheider auf (nicht nur zum Einkauf)</td></tr>
      <tr><td>2 → 3</td><td>Strategischer Partner</td><td>Initiiere regelmäßige Strategic Review Meetings, bringe Ideen proaktiv ein, zeige Wissen über die Branche des Kunden, spreche über seine Zukunft – nicht nur über dein Produkt</td></tr>
    </tbody>
  </table></div>

  <h3>Die White-Space-Analyse – systematisch Up-Selling-Potenziale finden</h3>
  <p>„White Space" sind die weißen Flecken auf der Karte: Standorte, Abteilungen, Tochtergesellschaften oder Produktbereiche deines Kunden, die du noch nicht bedienst. Ein aktives Key Account Management mappt diese systematisch.</p>
  <div class="tbl-wrap"><table>
    <thead><tr><th>Abteilung / Standort</th><th>Aktueller Status</th><th>Up-Sell-Potenzial</th><th>Barriere</th><th>Nächster Schritt</th></tr></thead>
    <tbody>
      <tr><td>Werk Nord (Stammwerk)</td><td><span class="badge bg">Hauptanlage aktiv ✅</span></td><td>IoT-Wartungsmodul (15.000 €)</td><td>Wartungsvertrag läuft Q3 aus</td><td>Review Meeting in Q2 ansetzen</td></tr>
      <tr><td>Werk Süd</td><td><span class="badge br">Mitbewerber ❌</span></td><td>Kompletttausch (~80.000 €)</td><td>Techn. Leiter unzufrieden mit Service</td><td>Intro über GF Nord anfordern</td></tr>
      <tr><td>Tochtergesellschaft Frankreich</td><td><span class="badge br">Kein System ❌</span></td><td>Adaption Konzept Werk Nord</td><td>GF Frankreich noch kein Kontakt</td><td>E-Mail-Intro über GF Deutschland</td></tr>
      <tr><td>Logistik-Hub Hamburg</td><td><span class="badge ba">Alte Anlage ⚠️</span></td><td>Modernisierung (~40.000 €)</td><td>Budget-Entscheidung im Q4</td><td>Jetzt platzieren für Q4-Budget</td></tr>
    </tbody>
  </table></div>

  <h3>Das Executive Review Meeting – der stärkste Up-Selling-Hebel</h3>
  <p>Up-Selling findet niemals „zwischen Tür und Angel" per Telefon statt. Du verpackst es immer in ein offizielles, strategisches Meeting auf Entscheider-Ebene – mit Ergebnissen, Daten und einem klaren Ausblick.</p>
  <div class="skript-box">
    <div class="sk-label">💬 Skript: Einladung zum Strategic Review Meeting</div>
    <div class="sk-text">„Herr/Frau [Name], Ihre Anlage läuft nun seit sechs Monaten stabil im Regelbetrieb – und ich freue mich, Ihnen mitteilen zu können, dass wir die gemeinsam gesetzten Effizienzziele im Werk Nord sogar um 4 % übertroffen haben.

Um sicherzustellen, dass wir diese Performance nicht nur halten, sondern auch mit Blick auf Ihre Expansionspläne für 2027 proaktiv weiterentwickeln, schlage ich ein kurzes, 30-minütiges Strategic Review Meeting vor.

Dort zeige ich Ihnen basierend auf unseren konkreten Learnings aus dem Werk Nord, wie wir die gleiche Effizienzsteigerung auch auf Ihr Werk Süd übertragen können – mit minimalem Implementierungsaufwand für Ihr Team, weil wir die Blaupause bereits haben.

Lassen Sie uns kurz die Kalender für die nächste Woche abgleichen. Wann hätten Sie 30 Minuten?"</div>
  </div>

  <h3>Up-Selling-Strategie 1: TCO Upgrade</h3>
  <p>Anstatt eine neue Investition zu fordern, zeige die Reduktion laufender Betriebskosten. Das Upgrade „verkauft sich selbst" wenn der ROI unter 12 Monate liegt.</p>
  <div class="skript-box">
    <div class="sk-label">💬 Skript: TCO Upgrade</div>
    <div class="sk-text">„Herr [Name], wir haben in unserer Analyse festgestellt, dass Ihre bestehende Anlage durch die manuellen Rüstzeiten jede Woche knapp 4 Stunden Stillstand produziert. Das entspricht einem kalkulatorischen Verlust von ca. 2.200 € pro Monat.

Wenn wir Ihr System auf das automatisierte Modul [X] upgraden, reduzieren wir diesen Stillstand auf unter 30 Minuten pro Woche. Die Investition: einmalig 15.000 €. Die Einsparung ab Monat 1: 2.200 €. Der Amortisationszeitpunkt: nach 7 Monaten.

Sollen wir die Modifikationen beim nächsten geplanten Wartungsfenster direkt mitinstallieren – dann haben Sie keine Extraausfallzeit?"</div>
  </div>

  <h3>Up-Selling-Strategie 2: Referenz-Skalierung</h3>
  <div class="skript-box">
    <div class="sk-label">💬 Skript: Referenz-Skalierung auf Tochtergesellschaft</div>
    <div class="sk-text">„Frau [Name], die Implementierung in Ihrer Logistikabteilung war ein voller Erfolg – Ihr Team spart dort aktuell 18 % der Bearbeitungszeit.

Da Sie im Konzern die Prozesse standardisieren wollen, macht es strategisch Sinn, diesen Best-Practice-Ansatz direkt auf die Produktion und den Einkauf auszuweiten.

Das Besondere: Wenn wir das jetzt replizieren, können wir das bestehende Schnittstellen-Setup eins zu eins übernehmen. Das spart Ihrer IT-Abteilung Wochen an Arbeit.

Wer ist in der Produktion der richtige Ansprechpartner, den wir am besten direkt mit ins Boot holen, um die Anforderungen zu definieren?"</div>
  </div>

  <h3>Das Empfehlungsmarketing auf C-Level – warme Leads ohne Kaltakquise</h3>
  <p>Der Magic Moment für eine Empfehlung ist immer nach dem ersten messbaren Erfolg – nie direkt nach Vertragsunterschrift. Dann bitte nicht mit einer generellen Frage, sondern mit einer gezielten, vorab recherchierten Person:</p>
  <div class="skript-box">
    <div class="sk-label">💬 Skript: Die geführte Empfehlungsfrage</div>
    <div class="sk-text">„Herr [Name], wir haben diese Woche die Leistungsdaten Ihres ersten Betriebsmonats ausgewertet – wir liegen bei einer Einsparung von 14 % über der ursprünglichen Kalkulation. Das zeigt, dass Ihre Entscheidung goldrichtig war.

Bei meiner Vorbereitung auf das heutige Gespräch habe ich gesehen, dass Sie auf LinkedIn mit Herrn [Name], dem Geschäftsführer der [Firmenname], vernetzt sind. Soweit ich weiß, steht die [Firmenname] vor einer ganz ähnlichen Herausforderung in ihren Werken.

Wie ist Ihr Draht zu Herrn [Name] – kennen Sie sich gut genug für eine kurze persönliche Einführung?"</div>
    <div class="sk-note">→ Biete an, den Einführungstext für den Kunden vorab zu schreiben. Er muss nur noch senden.</div>
  </div>

  <div class="aufgabe-box">
    <h4>📝 Praxis-Übung (7 Min.)</h4>
    <ol>
      <li>Wähle deine Top-3-Bestandskunden nach Umsatz. Auf welcher Stufe (1, 2 oder 3) befindet sich jede Beziehung?</li>
      <li>Erstelle für jeden eine White-Space-Analyse: Welche Standorte, Abteilungen oder Tochtergesellschaften nutzen unsere Lösung noch nicht?</li>
      <li>Formuliere die Einladung zum Executive Review Meeting für den vielversprechendsten Account und sende sie noch heute.</li>
    </ol>
  </div>

  <div class="nav-btns">
    <button class="btn" onclick="showMod(4)">← Zurück</button>
    <button class="btn btn-primary" onclick="nextMod(5)">Weiter: Preisverhandlung →</button>
  </div>
</div>
</div>

<!-- ══════════════════ MODULE 6: PREISVERHANDLUNG ══ -->
<div class="module" id="m6">
<div class="card">
  <div class="mod-title"><span class="mico">🛡️</span>Souveräne Preisverhandlung gegen professionelle Einkäufer</div>
  <p>Ein professioneller Einkäufer hat eine spezifische Ausbildung in Verhandlungstaktiken. Er kennt die Psychologie hinter Preisverhandlungen und nutzt diese systematisch. Bevor du in so ein Gespräch gehst, musst du seine Werkzeuge kennen – und deine Antworten vorbereitet haben.</p>
  <div class="highlight"><strong>Die goldene Regel: Es ist ein Theaterstück.</strong> „Ihr Angebot ist völlig indiskutabel" ist kein persönlicher Angriff und oft nicht einmal die Wahrheit – es ist seine Eröffnungsposition. Deine wichtigste Stärke: Der Fachbereich (z.B. der Produktionsleiter) hat sich bereits intern für dich entschieden. Der Einkauf soll nur noch das Beste aus dem Preis herausholen.</div>

  <h3>Das Machtgefüge verstehen – wer wirklich entscheidet</h3>
  <p>Im B2B gibt es immer zwei Entscheider: den <strong>Fachbereich</strong> (technischer Leiter, Produktionsleiter, Werkleiter) und den <strong>Einkauf</strong>. Der Fachbereich will deine Lösung – er hat sie intern bereits als beste Option identifiziert. Der Einkauf hat den Auftrag, den Preis zu drücken. Wenn du das weißt, kannst du viel souveräner verhandeln.</p>
  <div class="hl-blue"><strong>Dein stärkster Hebel:</strong> Der Fachbereich ist dein Champion. Im Zweifel kann er den Einkauf überstimmen, wenn dein Mehrwert klar genug kommuniziert ist. Baue im Gespräch immer Referenzen auf den Fachbereich ein: „Das haben wir gemeinsam mit Herrn [technischer Leiter] so erarbeitet – er hat das explizit als wichtiges Kriterium genannt."</div>

  <h3>Taktik 1: Die Salamitaktik – scheibchenweise Erosion</h3>
  <p><strong>Was der Einkäufer tut:</strong> Er tut so, als ob der Deal schon so gut wie sicher ist – und fordert dann, kurz vor der Unterschrift, immer noch eine weitere „Kleinigkeit". Gratis-Frachtkosten. Einen zusätzlichen Service-Tag. Eine längere Garantie ohne Aufpreis. Gibst du nach, kommt unweigerlich die nächste Kleinigkeit. So erodiert er deine Marge scheibchenweise.</p>
  <div class="skript-box">
    <div class="sk-label">💬 Elite-Konter: Das Paket-Prinzip</div>
    <div class="sk-text">„Herr [Name], wir können uns beim Thema Frachtkosten gerne bewegen – ich will das konstruktiv angehen. Wenn wir das machen, müssen wir aber das Gesamtpaket neu strukturieren.

Wenn wir die Transportlogistik auf unsere Kappe nehmen, erhöhen wir im Gegenzug die Anzahlung bei Auftragserteilung von 30 % auf 50 %, um unsere Projektliquidität zu sichern. Das ist für uns die einzige Art, wie das kaufmännisch funktioniert.

Sollen wir das Angebot in dieser Form anpassen – dann können Sie es heute noch freigeben?"</div>
    <div class="sk-note">→ Die eiserne Regel: Gib niemals etwas ohne Gegenleistung. Jedes einseitige Zugeständnis lädt zu weiteren Forderungen ein und signalisiert, dass du noch mehr Spielraum hast.</div>
  </div>

  <h3>Taktik 2: Die künstliche Deadline – Zeitdruck als Waffe</h3>
  <p><strong>Was der Einkäufer tut:</strong> Er setzt eine willkürliche Deadline: „Ich brauche Ihren finalen Tiefstpreis bis heute 16:00 Uhr, sonst gehen wir zum Mitbewerber." Das Ziel: Dich unter Zeitdruck zu setzen, damit du unüberlegt nachgibst ohne eine Gegenleistung einzufordern.</p>
  <p><strong>Was du nicht tust:</strong> Rennen. Wer unter Druck läuft, verliert sofort an Wert. Ein Anbieter, der bei Zeitdruck nachgibt, wird als schwach wahrgenommen – und als jemand, den man weiter drücken kann.</p>
  <div class="skript-box">
    <div class="sk-label">💬 Elite-Konter: Kühle Souveränität</div>
    <div class="sk-text">„Frau [Name], ich verstehe vollkommen, dass Sie das Projekt zügig zum Abschluss bringen möchten – das möchten wir auch.

Ich muss Ihnen aber transparent sagen: Unsere Kalkulation ist exakt auf die technischen Anforderungen abgestimmt, die Ihr Fachbereich als kritisch definiert hat – die Ausfallsicherheit, die Effizienzgarantie und die Servicezeiten. In diesem Budget ist kein Puffer für Preis-Runden eingebaut, weil er zulasten dieser Garantien gehen würde.

Wenn ich jetzt unter Zeitdruck den Preis reduziere, müsste ich Spezifikationen aus dem Lieferumfang nehmen – und das würde den Erfolg des Projekts gefährden. Das ist nicht in Ihrem Interesse und nicht in unserem.

Ich schlage vor: Wir lassen die Zahlen wie sie sind – und ich stelle sicher, dass wir administrativ alles beschleunigen was möglich ist. Was würden Sie brauchen um heute zu entscheiden?"</div>
  </div>

  <h3>Taktik 3: Das Anker-Prinzip – utopische Gegenforderungen</h3>
  <p><strong>Was der Einkäufer tut:</strong> Du hast 200.000 € angeboten. Er sagt kalt: „Bei 140.000 € können wir anfangen zu reden." Er setzt einen extrem niedrigen Anker – wissend, dass ihr euch in der Mitte (bei ~170.000 €) treffen werdet. Wenn du das mitmachst, hast du 30.000 € verloren.</p>
  <p><strong>Die Psychologie:</strong> Wer sich auf den Anker einlässt – egal wie tief – hat akzeptiert, dass der Anker-Wert eine legitime Ausgangsbasis ist. Der Anker muss sofort disqualifiziert werden.</p>
  <div class="skript-box">
    <div class="sk-label">💬 Elite-Konter: Den Anker disqualifizieren</div>
    <div class="sk-text">„Herr [Name], ich erkenne, dass Sie ein hartes Verhandlungsgespräch führen – das ist völlig legitim.

Aber lassen Sie mich direkt mit Ihnen sein: Eine Differenz von 60.000 € lässt sich nicht durch Verhandlungsgeschick erklären. Das ist kein Spielraum – das sind zwei fundamental verschiedene Lösungen mit verschiedenen Leistungsversprechen.

Wenn Ihr Budget wirklich bei 140.000 € gedeckelt ist, haben wir am Bedarf, den Ihr technisches Team uns kommuniziert hat, vorbeigeplant. Das tut mir leid – das sollten wir dann transparent machen.

Ich würde vorschlagen, wir stoppen kurz und ich stimme ab, was innerhalb von 140.000 € technisch noch lieferbar ist – aber dann mit einer deutlich anderen Effizienz und ohne die kritischen Redundanzen. Soll ich das intern kurz prüfen und Ihnen bis morgen eine ehrliche Alternative schicken?"</div>
    <div class="sk-note">→ Du disqualifizierst den Anker ohne ihn zu akzeptieren. Und du gibst dem Einkäufer eine Möglichkeit, aus der Sackgasse herauszukommen ohne sein Gesicht zu verlieren.</div>
  </div>

  <h3>Die „Wenn-Dann"-Matrix – dein Schutzschild gegen Margen-Erosion</h3>
  <p>Bereite diese Matrix vor jedem wichtigen Verhandlungsgespräch vor. Jede Forderung des Einkäufers hat eine vorbereitete Gegenleistung. Du gibst nie etwas ohne Kompensation.</p>
  <div class="tbl-wrap"><table>
    <thead><tr><th>Wenn der Einkäufer fordert …</th><th>… dann fordern wir als Gegenleistung</th><th>Warum das funktioniert</th></tr></thead>
    <tbody>
      <tr><td>„Wir brauchen 5% Nachlass."</td><td>Laufzeit des Wartungsvertrags von 12 auf 36 Monate verlängern</td><td>Planungssicherheit und Folgegeschäft für uns</td></tr>
      <tr><td>„Gehen Sie beim Preis runter."</td><td>Liefertermin um 4 Wochen nach hinten verlegen (Sommerloch nutzen)</td><td>Bessere Produktionsplanung auf unserer Seite</td></tr>
      <tr><td>„Das Budget reicht nicht."</td><td>Software-Schnittstelle [X] oder Feature [Y] aus Lieferumfang nehmen</td><td>Gleicher Preis, weniger Leistungsumfang – sauber</td></tr>
      <tr><td>„Geben Sie uns Skonto."</td><td>Zahlung innerhalb von 3 Werktagen nach Lieferung auf unserem Konto</td><td>Liquiditätsvorteil ist das Skonto wert</td></tr>
      <tr><td>„Wir brauchen längere Zahlungsziele (90 Tage)."</td><td>Abnahmemenge um mindestens 20–30 % erhöhen</td><td>Grösseres Volumen kompensiert Finanzierungskosten</td></tr>
      <tr><td>„Kostenlose Schulung inklusive."</td><td>Referenz-Case-Freigabe für unsere Marketing-Nutzung</td><td>Marketing-Wert schlägt den Schulungswert</td></tr>
    </tbody>
  </table></div>

  <h3>Dein Walk-Away-Point – wann du den Deal stehen lässt</h3>
  <p>Der Walk-Away-Point ist deine untere Grenze – der Punkt, unter dem du lieber keinen Deal machst als einen schlechten. Wer keinen definierten Walk-Away-Point hat, gibt immer nach. Definiere ihn vor jedem Gespräch:</p>
  <ul>
    <li><strong>Zielpreis:</strong> Der Preis den du anstrebst (dein Angebotspreis)</li>
    <li><strong>BATNA:</strong> Best Alternative to No Agreement – was passiert wenn der Deal nicht kommt?</li>
    <li><strong>Walk-Away-Point:</strong> Die unterste Grenze, unter der du abbrichst – und das sagst du dir selbst vor dem Gespräch</li>
  </ul>
  <div class="hl-amber"><strong>Die Paradoxie der Verhandlung:</strong> Wer bereit ist zu gehen, verhandelt am stärksten. Wenn der Einkäufer spürt, dass du den Deal unter allen Umständen brauchst, hat er alle Macht. Wenn er spürt, dass du auch ohne ihn leben kannst, respektiert er dich – und gibt nach.</div>

  <div class="aufgabe-box">
    <h4>📝 Praxis-Übung (7 Min.)</h4>
    <ol>
      <li>Definiere für dein nächstes Verhandlungsgespräch: Zielpreis, BATNA und Walk-Away-Point. Schreibe alle drei auf.</li>
      <li>Schreibe 3 Wenn-Dann-Paare, die du für diesen konkreten Deal einsetzen würdest.</li>
      <li>Übe den Anker-Konter laut vor dem Spiegel. Er muss ruhig und sachlich klingen – nicht defensiv oder beleidigt.</li>
    </ol>
  </div>

  <div class="nav-btns">
    <button class="btn" onclick="showMod(5)">← Zurück</button>
    <button class="btn btn-primary" onclick="nextMod(6)">Weiter: Abschlusstest →</button>
  </div>
</div>
</div>

<!-- ══════════════════ MODULE 7: ABSCHLUSSTEST ══ -->
<div class="module" id="m7">
<div class="card">
  <div class="mod-title"><span class="mico">🏆</span>Abschlusstest – 5 Elite-Fragen</div>
  <p>Diese 20 Fragen decken alle Module der B2B Sales Masterclass ab. Nur wer die Schulung wirklich verstanden hat, besteht. Bestehen = mindestens 16 von 20.</p>
</div>

<div class="card">
  <div class="name-row">
    <label for="qename">👤 Dein Name:</label>
    <input type="text" id="qename" placeholder="Vor- und Nachname eingeben …" autocomplete="name" />
  </div>
  <div class="prog-wrap">
    <div class="prog-meta">
      <span id="prog-text">0 von 20 beantwortet</span>
      <span id="prog-score-inner">0 richtig</span>
    </div>
    <div class="prog-bar"><div class="prog-fill" id="prog-fill"></div></div>
  </div>

  <div class="qblock" id="qb1">
    <div class="q-header"><span class="q-num">Frage 1 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Ein Einkäufer sagt: „Ihr Angebot ist 20 % teurer als das des Mitbewerbers!" Wie reagierst du?</div>
    <button class="opt" onclick="pick(this,1,'a')"><span class="dot"></span>Ich gebe ihm sofort 10 % Rabatt, um guten Willen zu zeigen</button>
    <button class="opt" onclick="pick(this,1,'b')"><span class="dot"></span>Ich frage, ob er die Anschaffungskosten oder die laufenden Betriebskosten (TCO) über die nächsten 5 Jahre minimieren will</button>
    <button class="opt" onclick="pick(this,1,'c')"><span class="dot"></span>Ich erkläre ihm lang und breit, warum unsere Komponenten qualitativ hochwertiger sind</button>
    <div class="fb ok" id="fb1ok">✓ Richtig! Die ROI-Umdrehung verlagert den Fokus vom Anschaffungspreis auf die Betriebskosten. Ein Sofortrabatt signalisiert, dass der Ursprungspreis gelogen war.</div>
    <div class="fb err" id="fb1err">✗ Richtig wäre B. Die ROI-Umdrehung: Fokus von Anschaffung auf TCO über 5 Jahre. Sofortiger Rabatt zerstört deine Glaubwürdigkeit dauerhaft.</div>
  </div>

  <div class="qblock" id="qb2">
    <div class="q-header"><span class="q-num">Frage 2 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Was ist das primäre Ziel der „Break-up-E-Mail" bei stagnierenden Deals?</div>
    <button class="opt" onclick="pick(this,2,'a')"><span class="dot"></span>Den Kunden zu bestrafen, weil er sich nicht meldet</button>
    <button class="opt" onclick="pick(this,2,'b')"><span class="dot"></span>Durch künstliche Verknappung und Verlustangst eine klare Entscheidung (Ja oder Nein) zu provozieren</button>
    <button class="opt" onclick="pick(this,2,'c')"><span class="dot"></span>Dem Chef zu zeigen, dass man die Pipeline aktiv pflegt</button>
    <div class="fb ok" id="fb2ok">✓ Richtig! Die Break-up-E-Mail triggert Loss Aversion. Ein Entscheider der das Projekt wirklich will, meldet sich sofort. Wenn nicht – war der Deal ohnehin tot.</div>
    <div class="fb err" id="fb2err">✗ Richtig wäre B. Das psychologische Prinzip: Verlustangst (Loss Aversion). Reservierte Ressourcen gehen verloren – das provoziert ehrliche Reaktionen.</div>
  </div>

  <div class="qblock" id="qb3">
    <div class="q-header"><span class="q-num">Frage 3 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Wann ist der perfekte Zeitpunkt (Magic Moment), um einen B2B-Kunden nach einer C-Level-Empfehlung zu fragen?</div>
    <button class="opt" onclick="pick(this,3,'a')"><span class="dot"></span>Direkt nach der Vertragsunterschrift beim Erstabschluss</button>
    <button class="opt" onclick="pick(this,3,'b')"><span class="dot"></span>Wenn das Angebot per E-Mail rausgeht</button>
    <button class="opt" onclick="pick(this,3,'c')"><span class="dot"></span>Sobald die Anlage im Regelbetrieb die ersten messbaren Erfolge für den Kunden geliefert hat</button>
    <div class="fb ok" id="fb3ok">✓ Perfekt! Erst wenn der Kunde Ergebnisse erlebt hat, ist eine Empfehlung für ihn ein Statussymbol. Zu früh fragen schwächt jede Empfehlung.</div>
    <div class="fb err" id="fb3err">✗ Richtig wäre C. Nach dem ersten Erfolg – nicht vorher. Eine Empfehlung ohne Ergebnis ist wertlos und kann sogar schaden.</div>
  </div>

  <div class="qblock" id="qb4">
    <div class="q-header"><span class="q-num">Frage 4 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Ein Kunde bringt den Einwand: „Das Budget ist aktuell komplett eingefroren." Was tust du als Erstes?</div>
    <button class="opt" onclick="pick(this,4,'a')"><span class="dot"></span>Ich akzeptiere das und rufe in sechs Monaten wieder an</button>
    <button class="opt" onclick="pick(this,4,'b')"><span class="dot"></span>Ich isoliere den Einwand: „Angenommen, das Budget wäre freigegeben – gäbe es dann noch andere Hürden?"</button>
    <button class="opt" onclick="pick(this,4,'c')"><span class="dot"></span>Ich biete ihm sofort eine Ratenzahlung an</button>
    <div class="fb ok" id="fb4ok">✓ Richtig! Immer erst isolieren, bevor man eine Lösung anbietet. Sonst behandelst du vielleicht den falschen Einwand.</div>
    <div class="fb err" id="fb4err">✗ Richtig wäre B. Isolation zuerst! Erst wenn Budget das einzige Hindernis ist, macht eine Finanzierungsoption Sinn.</div>
  </div>

  <div class="qblock" id="qb5">
    <div class="q-header"><span class="q-num">Frage 5 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Welche eiserne Regel gilt beim Versenden von Angeboten, um „Ghosting" zu verhindern?</div>
    <button class="opt" onclick="pick(this,5,'a')"><span class="dot"></span>Das Angebot muss immer freitags um 16:00 Uhr verschickt werden</button>
    <button class="opt" onclick="pick(this,5,'b')"><span class="dot"></span>Kein Angebot verlässt das Haus, ohne dass ein fester Folgetermin zur gemeinsamen Besprechung im Kalender verankert ist</button>
    <button class="opt" onclick="pick(this,5,'c')"><span class="dot"></span>Das Angebot muss mindestens 50 Seiten lang sein, um seriös zu wirken</button>
    <div class="fb ok" id="fb5ok">✓ Korrekt! Die „No-Offer-Without-Date"-Regel. Der 15-Minuten-Folgetermin ist dein Versicherungsschutz gegen das schwarze Loch.</div>
    <div class="fb err" id="fb5err">✗ Richtig wäre B. Kein Angebot ohne Datum. Erst der vereinbarte Folgetermin verhindert, dass du im E-Mail-Limbo versinkst.</div>
  </div>

  <div class="qblock" id="qb6">
    <div class="q-header"><span class="q-num">Frage 6 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Ein Kunde sagt: „Wir haben bereits einen festen Lieferanten und sind zufrieden." Was ist die stärkste Reaktion?</div>
    <button class="opt" onclick="pick(this,6,'a')"><span class="dot"></span>Den Wettbewerber direkt schlechtreden und technische Schwächen aufzeigen</button>
    <button class="opt" onclick="pick(this,6,'b')"><span class="dot"></span>Einen unverbindlichen Proof-of-Concept anbieten: „Wenn wir besser sind, haben Sie eine Alternative. Wenn nicht, haben Sie Gewissheit."</button>
    <button class="opt" onclick="pick(this,6,'c')"><span class="dot"></span>Das Gespräch beenden und erst in 3 Monaten wieder anrufen</button>
    <div class="fb ok" id="fb6ok">✓ Genau! Die Benchmark-Taktik. Du forderst keinen Wechsel – du bietest Absicherung an. Das senkt die wahrgenommene Risikobarriere auf null.</div>
    <div class="fb err" id="fb6err">✗ Richtig wäre B. Die Benchmark-Taktik: kein Wechsel gefordert, nur Vergleich. Wettbewerber schlechtreden zerstört Glaubwürdigkeit sofort.</div>
  </div>

  <div class="qblock" id="qb7">
    <div class="q-header"><span class="q-num">Frage 7 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Was bedeutet die LAEV-Abkürzung im Einwandbehandlungs-Framework?</div>
    <button class="opt" onclick="pick(this,7,'a')"><span class="dot"></span>Liefern – Angebot – Einwand – Vertrag</button>
    <button class="opt" onclick="pick(this,7,'b')"><span class="dot"></span>Lauschen – Anerkennen – Ergründen/Isolieren – Verändern/Lösen</button>
    <button class="opt" onclick="pick(this,7,'c')"><span class="dot"></span>Lead – Angebot – Entscheider – Verkauf</button>
    <div class="fb ok" id="fb7ok">✓ Richtig! L-A-E-V: Lauschen & Atmen → Anerkennen → Ergründen & Isolieren → Verändern & Lösen. Die Reihenfolge ist nicht verhandelbar.</div>
    <div class="fb err" id="fb7err">✗ Richtig wäre B. LAEV = Lauschen → Anerkennen → Ergründen/Isolieren → Verändern/Lösen. Das ist der 4-Schritt-Prozess für jeden Einwand.</div>
  </div>

  <div class="qblock" id="qb8">
    <div class="q-header"><span class="q-num">Frage 8 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Was ist der Unterschied zwischen einem echten Einwand und einem Vorwand?</div>
    <button class="opt" onclick="pick(this,8,'a')"><span class="dot"></span>Ein Vorwand ist aggressiver formuliert als ein echter Einwand</button>
    <button class="opt" onclick="pick(this,8,'b')"><span class="dot"></span>Ein Vorwand ist ein vorgeschobener Grund, der den wahren Hinderungsgrund verdeckt – z. B. „kein Budget" obwohl der echte Grund fehlendes ROI-Verständnis ist</button>
    <button class="opt" onclick="pick(this,8,'c')"><span class="dot"></span>Es gibt keinen Unterschied – alle Einwände müssen gleich behandelt werden</button>
    <div class="fb ok" id="fb8ok">✓ Perfekt! Vorwände verbergen den echten Einwand. Deshalb immer erst isolieren mit der Frage: „Angenommen, das wäre kein Thema – gibt es noch andere Gründe?"</div>
    <div class="fb err" id="fb8err">✗ Richtig wäre B. Vorwände sind Schutzschilde. Den echten Einwand findest du nur durch gezielte Isolation – nie durch direkte Behandlung des Vorwands.</div>
  </div>

  <div class="qblock" id="qb9">
    <div class="q-header"><span class="q-num">Frage 9 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Was ist der „Cost of Inaction" und wann setzt du dieses Closing-Framework ein?</div>
    <button class="opt" onclick="pick(this,9,'a')"><span class="dot"></span>Die Kosten der Implementierung – einsetzen um den Preis zu rechtfertigen</button>
    <button class="opt" onclick="pick(this,9,'b')"><span class="dot"></span>Die monatlichen Verluste durch Nicht-Handeln – einsetzen wenn ein Kunde die Entscheidung verschieben will</button>
    <button class="opt" onclick="pick(this,9,'c')"><span class="dot"></span>Die Konkurrenzkosten – einsetzen beim Preisvergleich</button>
    <div class="fb ok" id="fb9ok">✓ Richtig! Menschen reagieren doppelt so stark auf Verlust wie auf Gewinn. „Jedes weitere Monat kostet Sie X €" ist stärker als jedes Gewinn-Argument.</div>
    <div class="fb err" id="fb9err">✗ Richtig wäre B. Cost of Inaction = die laufenden Verluste durch den Ist-Zustand. Ideal gegen Aufschieberitis: „Das Warten kostet Sie 6.500 € pro Monat."</div>
  </div>

  <div class="qblock" id="qb10">
    <div class="q-header"><span class="q-num">Frage 10 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Ein Einkäufer übt mit einer utopisch niedrigen Gegenforderung Druck aus (Anker-Prinzip). Dein Angebot: 200.000 €. Er sagt: „Bei 140.000 € fangen wir an." Was tust du?</div>
    <button class="opt" onclick="pick(this,10,'a')"><span class="dot"></span>Ich treffe mich in der Mitte bei 170.000 €, um den Deal zu retten</button>
    <button class="opt" onclick="pick(this,10,'b')"><span class="dot"></span>Ich zerstöre den Anker sofort: „Eine Differenz von 60.000 € ist kein Verhandlungsspielraum – das sind zwei verschiedene technologische Lösungen. Wollen wir das Projekt neu konzipieren?"</button>
    <button class="opt" onclick="pick(this,10,'c')"><span class="dot"></span>Ich biete 190.000 € als Kompromiss an und hoffe auf Zustimmung</button>
    <div class="fb ok" id="fb10ok">✓ Korrekt! Den Anker zerstören statt akzeptieren. Wer sich auf den Ankerwert einlässt, hat das Verhandlungsrahmen verloren. Das 60.000-€-Gap ist keine Verhandlungsfrage, sondern eine Produktfrage.</div>
    <div class="fb err" id="fb10err">✗ Richtig wäre B. Den Anker sofort disqualifizieren. Wer sich in der Mitte trifft, gibt zu, dass der Originalpreis falsch war. Das signalisiert: Ich kann noch weiter gedrückt werden.</div>
  </div>

  <div class="qblock" id="qb11">
    <div class="q-header"><span class="q-num">Frage 11 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Was ist das Konzept der „Schulter-an-Schulter"-Positionierung im B2B-Closing?</div>
    <button class="opt" onclick="pick(this,11,'a')"><span class="dot"></span>Dem Kunden körperlich nahe sein – Augenkontakt und Körpersprache einsetzen</button>
    <button class="opt" onclick="pick(this,11,'b')"><span class="dot"></span>Man sitzt virtuell neben dem Kunden als strategischer Berater der sein Problem löst – nicht gegenüber als Verkäufer der Geld will</button>
    <button class="opt" onclick="pick(this,11,'c')"><span class="dot"></span>Immer zu zweit in Kundengespräche gehen, um Druck aufzubauen</button>
    <div class="fb ok" id="fb11ok">✓ Perfekt! Das ist das Kern-Mindset. Wenn du als strategischer Partner wahrgenommen wirst, wird das Closing zur logischen Konsequenz – nicht zum verkäuferischen Druck.</div>
    <div class="fb err" id="fb11err">✗ Richtig wäre B. Positionierung als Berater, nicht als Verkäufer. Closing ist dann ein gemeinsames Festlegen der nächsten Schritte, kein Überreden.</div>
  </div>

  <div class="qblock" id="qb12">
    <div class="q-header"><span class="q-num">Frage 12 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Was ist die „Salamitaktik" eines Einkäufers – und wie konterst du sie?</div>
    <button class="opt" onclick="pick(this,12,'a')"><span class="dot"></span>Der Einkäufer schneidet das Gespräch kurz ab – Konter: mehr Zeit einfordern</button>
    <button class="opt" onclick="pick(this,12,'b')"><span class="dot"></span>Der Einkäufer fordert kurz vor Unterschrift immer neue „Kleinigkeiten" – Konter: Paket-Prinzip – jedes Zugeständnis wird mit einer Gegenleistung verknüpft</button>
    <button class="opt" onclick="pick(this,12,'c')"><span class="dot"></span>Der Einkäufer verhandelt in sehr kleinen Schritten – Konter: sofort den Endpreis nennen</button>
    <div class="fb ok" id="fb12ok">✓ Richtig! Die Salamitaktik zielt auf schrittweise Erosion der Marge. Konter: Paket-Prinzip. „Wenn wir bei X nachgeben, brauchen wir bei Y eine Gegenleistung." Niemals einseitig geben.</div>
    <div class="fb err" id="fb12err">✗ Richtig wäre B. Salamitaktik = scheibchenweise Forderungen kurz vor Abschluss. Konter: Das Paket-Prinzip – keine Konzession ohne Gegenforderung.</div>
  </div>

  <div class="qblock" id="qb13">
    <div class="q-header"><span class="q-num">Frage 13 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Auf welcher Abschluss-Wahrscheinlichkeit bewertest du einen Deal, bei dem das Angebot verhandelt und alle Einwände isoliert wurden?</div>
    <button class="opt" onclick="pick(this,13,'a')"><span class="dot"></span>10 % – man weiß nie was passiert</button>
    <button class="opt" onclick="pick(this,13,'b')"><span class="dot"></span>60 % – Phase 3: Angebot verhandelt & Einwände isoliert</button>
    <button class="opt" onclick="pick(this,13,'c')"><span class="dot"></span>90 % – wenn er verhandelt, will er es sowieso</button>
    <div class="fb ok" id="fb13ok">✓ Richtig! Phase 3 im Pipeline-Modell = 60%. Phase 4 (finale Abstimmung) = 90%. Diese Gewichtung verhindert Pipeline-Illusion und ermöglicht realistische Umsatzplanung.</div>
    <div class="fb err" id="fb13err">✗ Richtig wäre B. Phase 3 = 60%. Nur Phase 4 (Einkaufsschleife läuft) = 90%. Zu optimistisch denken führt zur Pipeline-Illusion und falschen Quartalsprognosen.</div>
  </div>

  <div class="qblock" id="qb14">
    <div class="q-header"><span class="q-num">Frage 14 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Du willst 500.000 € Jahresumsatz erzielen. Dein durchschnittlicher Deal-Wert beträgt 50.000 €, deine Abschlussquote ab Angebot 25 %. Wie viele Angebote musst du im Jahr legen?</div>
    <button class="opt" onclick="pick(this,14,'a')"><span class="dot"></span>10 Angebote</button>
    <button class="opt" onclick="pick(this,14,'b')"><span class="dot"></span>40 Angebote</button>
    <button class="opt" onclick="pick(this,14,'c')"><span class="dot"></span>100 Angebote</button>
    <div class="fb ok" id="fb14ok">✓ Richtig! 500.000 € / 50.000 € = 10 Abschlüsse nötig. Bei 25% Quote: 10 / 0,25 = 40 Angebote. Rückwärtsrechnen macht das Ziel greifbar und planbar.</div>
    <div class="fb err" id="fb14err">✗ Richtig wäre B. Rechnung: 500.000 € / 50.000 € = 10 Abschlüsse. Bei 25% Abschlussquote: 10 × 4 = 40 Angebote. Das ist deine Jahresaufgabe – heruntergebrochen pro Woche.</div>
  </div>

  <div class="qblock" id="qb15">
    <div class="q-header"><span class="q-num">Frage 15 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Ein Einkäufer setzt eine künstliche Deadline: „Ich brauche Ihren finalen Tiefstpreis bis heute 16 Uhr, sonst fliegen Sie aus dem Tender." Was ist die richtige Reaktion?</div>
    <button class="opt" onclick="pick(this,15,'a')"><span class="dot"></span>Sofort reagieren und den Preis um 5 % senken, um den Deal zu retten</button>
    <button class="opt" onclick="pick(this,15,'b')"><span class="dot"></span>Ruhig bleiben und erklären: In der Kalkulation ist kein Spielraum für Rabatt-Runden eingebaut – Qualitätsreduktion wäre die Konsequenz, keine Preissenkung</button>
    <button class="opt" onclick="pick(this,15,'c')"><span class="dot"></span>Um einen Tag Verlängerung bitten und intern Rabattgrenzen klären</button>
    <div class="fb ok" id="fb15ok">✓ Korrekt! Wer rennt, verliert Wert. Kühle Souveränität statt Hektik. Die Deadline ist ein Druckmittel – kein echtes Kriterium. Qualität schützen ist stärker als Preisnachgeben.</div>
    <div class="fb err" id="fb15err">✗ Richtig wäre B. Kühle Souveränität. Wer unter Zeitdruck nachgibt, zeigt: Mein Originalpreis war nicht vertretbar. Das lädt zu weiteren Druckversuchen ein.</div>
  </div>

  <div class="qblock" id="qb16">
    <div class="q-header"><span class="q-num">Frage 16 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Was ist das „Alternative / Conditional Closing" – und welchen psychologischen Effekt erzeugt es?</div>
    <button class="opt" onclick="pick(this,16,'a')"><span class="dot"></span>Du gibst dem Kunden zwei Preisvarianten zur Wahl, um ihn zu einem Kauf zu zwingen</button>
    <button class="opt" onclick="pick(this,16,'b')"><span class="dot"></span>Du gibst dem Kunden die Kontrolle über das WIE (DocuSign oder Rechtsabteilung), nicht über das OB – das reduziert das Gefühl eingesperrt zu sein</button>
    <button class="opt" onclick="pick(this,16,'c')"><span class="dot"></span>Du bietest eine Alternative an, falls der Hauptdeal scheitert</button>
    <div class="fb ok" id="fb16ok">✓ Perfekt! Der psychologische Effekt: Autonomiegefühl. Der Kunde entscheidet über den Prozess, nicht ob er kauft. Das senkt Abwehr bei gleichzeitiger Verbindlichkeit.</div>
    <div class="fb err" id="fb16err">✗ Richtig wäre B. Das Conditional Closing gibt Kontrolle über das WIE, nicht das OB. Das erzeugt Autonomiegefühl und senkt Entscheidungsabwehr gleichzeitig.</div>
  </div>

  <div class="qblock" id="qb17">
    <div class="q-header"><span class="q-num">Frage 17 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Ab welcher Inaktivitätsdauer sollte ein Deal in deinem CRM die Break-up-E-Mail erhalten?</div>
    <button class="opt" onclick="pick(this,17,'a')"><span class="dot"></span>Nach 6 Monaten ohne Reaktion</button>
    <button class="opt" onclick="pick(this,17,'b')"><span class="dot"></span>Nach 2 Wochen ohne Reaktion trotz Nachfass-Protokoll</button>
    <button class="opt" onclick="pick(this,17,'c')"><span class="dot"></span>Erst wenn der Kunde selbst absagt</button>
    <div class="fb ok" id="fb17ok">✓ Richtig! 2 Wochen nach dem letzten Kontaktversuch. Schnelles „Nein" ist besser als ein langsames „Vielleicht". Karteileichen blockieren deine mentale Energie für echte Deals.</div>
    <div class="fb err" id="fb17err">✗ Richtig wäre B. Nach 2 Wochen ohne Reaktion. 6 Monate warten ist Pipeline-Illusion. Schnelles Nein schafft Klarheit und freie Kapazität für heiße Leads.</div>
  </div>

  <div class="qblock" id="qb18">
    <div class="q-header"><span class="q-num">Frage 18 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Auf welcher Entwicklungsstufe einer Kundenbeziehung wirst du VOR der Budgetplanung an den Tisch geholt?</div>
    <button class="opt" onclick="pick(this,18,'a')"><span class="dot"></span>Stufe 1: Transaktions-Lieferant</button>
    <button class="opt" onclick="pick(this,18,'b')"><span class="dot"></span>Stufe 3: Strategischer Partner</button>
    <button class="opt" onclick="pick(this,18,'c')"><span class="dot"></span>Stufe 2: Bevorzugter Anbieter</button>
    <div class="fb ok" id="fb18ok">✓ Genau! Stufe 3 – Strategischer Partner. Der Kunde teilt seine 5-Jahres-Strategie. Austauschbarkeit: nahezu null. Das ist der Unterschied zwischen 30% und 70% Abschlusswahrscheinlichkeit pro Konto.</div>
    <div class="fb err" id="fb18err">✗ Richtig wäre B, Stufe 3. Nur als Strategischer Partner wirst du vor der Budgetplanung eingebunden. Stufe 2 ist gut – aber du wirst immer noch reaktiv angefragt, nicht proaktiv einbezogen.</div>
  </div>

  <div class="qblock" id="qb19">
    <div class="q-header"><span class="q-num">Frage 19 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Du willst einen Bestandskunden für ein Up-Selling-Gespräch gewinnen. Welches Format ist dafür am stärksten?</div>
    <button class="opt" onclick="pick(this,19,'a')"><span class="dot"></span>Eine kurze E-Mail mit dem neuen Produktkatalog und Preisliste</button>
    <button class="opt" onclick="pick(this,19,'b')"><span class="dot"></span>Ein 30-minütiges Strategic Review Meeting auf Entscheider-Ebene – auf Basis messbarer Ergebnisse der Bestandsinstallation</button>
    <button class="opt" onclick="pick(this,19,'c')"><span class="dot"></span>Ein Telefonat zwischen Tür und Angel, weil Bestandskunden keine formalen Termine brauchen</button>
    <div class="fb ok" id="fb19ok">✓ Richtig! Up-Selling im B2B läuft niemals nebenbei. Das Strategic Review Meeting schafft den Rahmen, in dem Ergebnisse präsentiert und Erweiterungspotenziale als logischer nächster Schritt erscheinen.</div>
    <div class="fb err" id="fb19err">✗ Richtig wäre B. Strategic Review Meeting. Up-Selling „zwischen Tür und Angel" signalisiert mangelnde Wertschätzung und führt zu schwachen Abschlussquoten bei Bestandskunden.</div>
  </div>

  <div class="qblock" id="qb20">
    <div class="q-header"><span class="q-num">Frage 20 von 20</span><span class="bdg bdg-h">Elite</span></div>
    <div class="qtext">Was signalisierst du einem Einkäufer, wenn du einen Rabatt gibst, ohne eine Gegenforderung zu stellen?</div>
    <button class="opt" onclick="pick(this,20,'a')"><span class="dot"></span>Partnerschaftlichkeit und guten Willen – das stärkt die Beziehung</button>
    <button class="opt" onclick="pick(this,20,'b')"><span class="dot"></span>Entweder dass du vorher zu teuer warst (gelogen) oder dass du schwach bist und weiter gedrückt werden kannst</button>
    <button class="opt" onclick="pick(this,20,'c')"><span class="dot"></span>Dass dein Produkt nicht den vollen Preis wert ist</button>
    <div class="fb ok" id="fb20ok">✓ Korrekt! Einseitiges Nachgeben ohne Gegenleistung ist das teuerste Signal das du senden kannst. Es öffnet die Tür für weitere Forderungen und zerstört langfristig deine Margenstruktur.</div>
    <div class="fb err" id="fb20err">✗ Richtig wäre B. Einseitiger Rabatt = „Ich war vorher nicht ehrlich" ODER „Ich bin schwach". Beides lädt zu weiteren Angriffen ein. Immer die Wenn-Dann-Formel nutzen.</div>
  </div>

  <div class="score-box" id="scorebox">
    <div class="score-val" id="scoreval">0</div>
    <div class="score-pct" id="scorepct">von 20 Fragen richtig</div>
    <div class="score-verdict" id="score-verdict">—</div>
    <div class="score-comment" id="scorecomment"></div>
    <div id="missedbox" style="display:none">
      <div class="missed-wrap">
        <div class="missed-title">Noch einmal anschauen:</div>
        <div id="missedlist"></div>
      </div>
    </div>
    <div class="btn-row">
      <button class="btn btn-primary" id="mailbtn" onclick="sendMail()" disabled>✉ Ergebnis an Chef senden</button>
      <button class="btn" onclick="resetTest()">↺ Test wiederholen</button>
    </div>
    <div class="mail-note" id="mailnote"></div>
  </div>

  <div class="nav-btns">
    <button class="btn" onclick="showMod(6)">← Zurück zu Modul 7</button>
    <div></div>
  </div>
</div>

<div class="card" style="background:linear-gradient(135deg,#071f38,#1A6B4A);color:#fff;margin-top:1rem">
  <div style="text-align:center;padding:1rem 0">
    <div style="font-size:40px;margin-bottom:.75rem">🎓</div>
    <h2 style="font-size:20px;font-weight:800;margin-bottom:.5rem;color:#fff">B2B Sales Masterclass abgeschlossen!</h2>
    <p style="opacity:.8;font-size:14px;max-width:480px;margin:0 auto .875rem">Du kennst jetzt die Elite-Frameworks für Einwandbehandlung, Closing, Key Account Management und Preisverhandlung. Geh raus und schließ ab.</p>
    <div style="display:flex;gap:12px;justify-content:center;flex-wrap:wrap">
      <button class="btn" style="background:rgba(255,255,255,.15);color:#fff;border-color:rgba(255,255,255,.3)" onclick="showMod(0)">↺ Von vorne beginnen</button>
    </div>
  </div>
</div>
</div>

</div><!-- /wrapper -->

<div class="footer">
  Realm Germany GmbH · B2B Sales Masterclass 2025 · Vertraulich · Nicht zur externen Weitergabe
</div>

<script>
/* ── MODULE NAVIGATION ── */
var modDone = {};
var curMod  = 0;
var MODS    = 8;

function showMod(n) {
  document.querySelectorAll('.module').forEach(function(m){ m.classList.remove('active'); });
  document.querySelectorAll('.nav-btn').forEach(function(b){ b.classList.remove('active'); });
  document.getElementById('m' + n).classList.add('active');
  document.getElementById('nc' + n).classList.add('active');
  curMod = n;
  window.scrollTo({ top: 0, behavior: 'smooth' });
  updateHeaderProgress();
}

function nextMod(n) {
  markModDone(n);
  showMod(n + 1);
}

function markModDone(n) {
  modDone[n] = true;
  var nb = document.getElementById('nc' + n);
  nb.classList.add('done');
  if (!nb.querySelector('.ncheck')) {
    var c = document.createElement('div');
    c.className = 'ncheck';
    c.textContent = '✓ Abgeschlossen';
    nb.appendChild(c);
  }
  updateHeaderProgress();
}

function updateHeaderProgress() {
  var done = Object.keys(modDone).length;
  var pct  = Math.round(done / MODS * 100);
  document.getElementById('hprog').style.width = pct + '%';
  document.getElementById('h-mod-txt').textContent = 'Modul ' + (curMod + 1) + ' von ' + MODS;
  document.getElementById('h-prog-txt').textContent = pct + ' % abgeschlossen';
}

/* ── MODULE MINI QUIZZES ── */
var mqCorrect = { 'm0q1':'b', 'm1q1':'b' };

function mqPick(el, qid, answer) {
  var block = el.parentElement;
  if (block.dataset.locked) return;
  block.dataset.locked = '1';
  block.querySelectorAll('.mopt').forEach(function(o){ o.style.pointerEvents = 'none'; });
  var isCorrect = answer === mqCorrect[qid];
  el.classList.add(isCorrect ? 'correct' : 'wrong');
  if (!isCorrect) {
    var opts = block.querySelectorAll('.mopt');
    ['a','b','c'].forEach(function(k, i){ if (k === mqCorrect[qid] && opts[i]) opts[i].classList.add('correct'); });
  }
  document.getElementById('mq-' + qid + '-ok').className = 'mfb ok' + (isCorrect ? ' show' : '');
  document.getElementById('mq-' + qid + '-err').className = 'mfb err' + (isCorrect ? '' : ' show');
}

/* ── FINAL TEST ── */
var correct = {1:'b',2:'b',3:'c',4:'b',5:'b',6:'b',7:'b',8:'b',9:'b',10:'b',11:'b',12:'b',13:'b',14:'b',15:'b',16:'b',17:'b',18:'b',19:'b',20:'b'};

var labels = {
  1:'Frage 1 – Reaktion auf Preisvergleich (ROI-Umdrehung)',
  2:'Frage 2 – Ziel der Break-up-E-Mail (Loss Aversion)',
  3:'Frage 3 – Magic Moment für C-Level-Empfehlung',
  4:'Frage 4 – Einwand „Budget eingefroren" (Isolation zuerst)',
  5:'Frage 5 – No-Offer-Without-Date-Regel',
  6:'Frage 6 – Einwand „fester Lieferant" (Benchmark-Taktik)',
  7:'Frage 7 – Das LAEV-Framework (Bedeutung der Abkürzung)',
  8:'Frage 8 – Einwand vs. Vorwand (Definition)',
  9:'Frage 9 – Cost of Inaction (Definition & Einsatz)',
  10:'Frage 10 – Anker-Prinzip des Einkäufers (Konter)',
  11:'Frage 11 – Schulter-an-Schulter-Positionierung',
  12:'Frage 12 – Salamitaktik des Einkäufers (Konter: Paket-Prinzip)',
  13:'Frage 13 – Pipeline-Wahrscheinlichkeit Phase 3 (60%)',
  14:'Frage 14 – KPI-Rückwärtsrechnung (40 Angebote für 500k €)',
  15:'Frage 15 – Künstliche Deadline des Einkäufers (Souveränität)',
  16:'Frage 16 – Alternative/Conditional Closing (Autonomieeffekt)',
  17:'Frage 17 – Break-up-E-Mail Timing (nach 2 Wochen)',
  18:'Frage 18 – Stufe 3: Strategischer Partner (vor Budgetplanung)',
  19:'Frage 19 – Up-Selling Format (Strategic Review Meeting)',
  20:'Frage 20 – Rabatt ohne Gegenleistung (Schwächesignal)'
};

var optTexts = {
  1:{a:'Sofort 10% Rabatt geben',b:'Frage: Anschaffungskosten oder TCO über 5 Jahre minimieren?',c:'Lange Qualitätserklärung ohne Zahlen'},
  2:{a:'Kunden bestrafen',b:'Verlustangst triggern – klare Entscheidung erzwingen (Loss Aversion)',c:'Pipeline-Pflege für den Chef dokumentieren'},
  3:{a:'Direkt nach Vertragsunterschrift',b:'Wenn das Angebot per E-Mail rausgeht',c:'Nach ersten messbaren Erfolgen im Regelbetrieb'},
  4:{a:'Akzeptieren und in 6 Monaten anrufen',b:'Isolationsfrage: „Angenommen Budget wäre frei – weitere Hürden?"',c:'Sofort Ratenzahlung anbieten'},
  5:{a:'Angebot immer freitags 16 Uhr',b:'Kein Angebot ohne festen Folgetermin zur gemeinsamen Besprechung',c:'Angebot muss 50+ Seiten lang sein'},
  6:{a:'Wettbewerber direkt schlechtreden',b:'Unverbindlichen Proof-of-Concept anbieten (Benchmark-Taktik)',c:'Gespräch beenden und in 3 Monaten anrufen'},
  7:{a:'Liefern – Angebot – Einwand – Vertrag',b:'Lauschen – Anerkennen – Ergründen/Isolieren – Verändern/Lösen',c:'Lead – Angebot – Entscheider – Verkauf'},
  8:{a:'Vorwand ist aggressiver formuliert',b:'Vorwand verbirgt den echten Einwand – z.B. „kein Budget" statt „kein ROI-Verständnis"',c:'Kein Unterschied – gleich behandeln'},
  9:{a:'Kosten der Implementierung – zur Preisrechtfertigung',b:'Monatliche Verluste durch Nicht-Handeln – bei Aufschieberitis einsetzen',c:'Konkurrenzkosten – beim Preisvergleich'},
  10:{a:'In der Mitte bei 170.000 € treffen',b:'Anker zerstören: „60.000 € Differenz = zwei verschiedene Lösungen – kein Verhandlungsspielraum"',c:'190.000 € als Kompromiss anbieten'},
  11:{a:'Körperlich nahesein und Augenkontakt',b:'Virtuell neben dem Kunden als Berater sitzen, nicht gegenüber als Verkäufer',c:'Immer zu zweit in Kundengespräche gehen'},
  12:{a:'Einkäufer bricht Gespräch ab – mehr Zeit einfordern',b:'Scheibchenweise Forderungen kurz vor Unterschrift – Konter: Paket-Prinzip (Gegenleistung)',c:'Sehr kleine Verhandlungsschritte – Endpreis sofort nennen'},
  13:{a:'10% – man weiß nie was passiert',b:'60% – Phase 3: Angebot verhandelt & Einwände isoliert',c:'90% – wenn er verhandelt, will er es sowieso'},
  14:{a:'10 Angebote',b:'40 Angebote',c:'100 Angebote'},
  15:{a:'Sofort 5% Preissenkung um Deal zu retten',b:'Kühle Souveränität: Kalkulation hat keinen Rabattspielraum – Qualitätsreduktion wäre die Konsequenz',c:'Um einen Tag Verlängerung bitten'},
  16:{a:'Zwei Preisvarianten zur Wahl geben',b:'Kontrolle über das WIE (DocuSign oder Rechtsabteilung) – nicht über das OB',c:'Alternative für den Fall eines Scheiterns anbieten'},
  17:{a:'Nach 6 Monaten ohne Reaktion',b:'Nach 2 Wochen ohne Reaktion trotz Nachfass-Protokoll',c:'Erst wenn der Kunde selbst absagt'},
  18:{a:'Stufe 1: Transaktions-Lieferant',b:'Stufe 3: Strategischer Partner',c:'Stufe 2: Bevorzugter Anbieter'},
  19:{a:'E-Mail mit Produktkatalog und Preisliste',b:'30-minütiges Strategic Review Meeting auf Entscheider-Ebene mit messbaren Ergebnissen',c:'Telefonat zwischen Tür und Angel'},
  20:{a:'Partnerschaftlichkeit und guten Willen signalisieren',b:'Entweder: „Ich war vorher zu teuer" ODER: „Ich bin schwach und kann weiter gedrückt werden"',c:'Dass das Produkt nicht den vollen Preis wert ist'}
};

var testAnswers = {};
var testLocked  = {};
var testAnswered = 0;
var testScore   = 0;
var TOTAL = 20;
var PASS  = 16;

function pick(el, qnum, answer) {
  if (testLocked[qnum]) return;
  testLocked[qnum] = true;
  var isCorrect = answer === correct[qnum];
  testAnswers[qnum] = { chosen: answer, correct: isCorrect };
  testAnswered++;
  if (isCorrect) testScore++;

  var block = document.getElementById('qb' + qnum);
  block.querySelectorAll('.opt').forEach(function(o){ o.classList.add('locked'); });
  el.classList.add(isCorrect ? 'correct' : 'wrong');
  if (!isCorrect) {
    block.querySelectorAll('.opt').forEach(function(o, i){
      if (['a','b','c'][i] === correct[qnum]) o.classList.add('correct');
    });
  }
  document.getElementById('fb' + qnum + 'ok').className = 'fb ok' + (isCorrect ? ' show' : '');
  document.getElementById('fb' + qnum + 'err').className = 'fb err' + (isCorrect ? '' : ' show');

  var pct = Math.round(testAnswered / TOTAL * 100);
  document.getElementById('prog-fill').style.width = pct + '%';
  document.getElementById('prog-text').textContent = testAnswered + ' von ' + TOTAL + ' beantwortet';
  document.getElementById('prog-score-inner').textContent = testScore + ' richtig';

  if (testAnswered === TOTAL) showScore();
}

function showScore() {
  var score  = testScore;
  var pct    = Math.round(score / TOTAL * 100);
  var passed = score >= PASS;

  document.getElementById('scoreval').textContent = score;
  document.getElementById('scoreval').className = 'score-val' + (passed ? '' : ' fail');
  document.getElementById('scorepct').textContent = 'von 20 Fragen richtig (' + pct + ' %) – Bestehen ab 16/20';

  var vd = document.getElementById('score-verdict');
  vd.textContent = passed ? '✓ ZERTIFIZIERT' : '✗ NICHT BESTANDEN';
  vd.className = 'score-verdict ' + (passed ? 'vpass' : 'vfail');

  var cmts = {
    20:'Perfekt – alle 20 Fragen richtig. B2B Sales Masterclass vollständig zertifiziert! 🏆',
    19:'Ausgezeichnet – 19/20. Winzige Lücke, sonst komplett.',
    18:'Sehr gut – 18/20. Zwei Module nochmal kurz anschauen.',
    17:'Gut – 17/20. Knapp über der Linie. Feinjustierung empfohlen.',
    16:'Bestanden – 16/20. Solide Basis. Einzelne Themen vertiefen.'
  };
  var comment = cmts[score] || (score < 16 ? 'Nicht bestanden – ' + score + '/20. Vollständige Wiederholung der schwachen Module empfohlen.' : '');
  document.getElementById('scorecomment').textContent = comment;
  document.getElementById('scorecomment').style.color = passed ? '#374151' : '#DC2626';

  var missed = [];
  for (var i = 1; i <= TOTAL; i++) {
    if (testAnswers[i] && !testAnswers[i].correct) missed.push(labels[i]);
  }
  if (missed.length > 0) {
    var ml = document.getElementById('missedlist');
    ml.innerHTML = '';
    missed.forEach(function(m){
      var d = document.createElement('div');
      d.className = 'missed-item';
      d.textContent = m;
      ml.appendChild(d);
    });
    document.getElementById('missedbox').style.display = 'block';
  }

  document.getElementById('scorebox').className = 'score-box show';
  markModDone(7);

  var name = document.getElementById('qename').value.trim();
  var btn  = document.getElementById('mailbtn');
  btn.disabled = !name;
  setMailNote(name);

  document.getElementById('qename').addEventListener('input', function(){
    var n = this.value.trim();
    btn.disabled = !n;
    setMailNote(n);
  });
}

function setMailNote(name) {
  var note = document.getElementById('mailnote');
  note.className = 'mail-note';
  note.textContent = name ? '' : 'Bitte trage deinen Namen ein, damit die E-Mail korrekt adressiert wird.';
}

function sendMail() {
  var name = document.getElementById('qename').value.trim();
  if (!name) { document.getElementById('mailnote').textContent = 'Bitte trage deinen Namen ein.'; return; }
  var score  = testScore;
  var pct    = Math.round(score / TOTAL * 100);
  var passed = score >= PASS ? 'BESTANDEN / ZERTIFIZIERT' : 'NICHT BESTANDEN';
  var now    = new Date();
  var ds     = now.toLocaleDateString('de-DE', {day:'2-digit', month:'2-digit', year:'numeric'});
  var ts     = now.toLocaleTimeString('de-DE', {hour:'2-digit', minute:'2-digit'});

  var lines = [];
  lines.push('ERGEBNISBERICHT – REALM GERMANY B2B SALES MASTERCLASS (20 FRAGEN)');
  lines.push('');
  lines.push('Mitarbeiter:  ' + name);
  lines.push('Datum:        ' + ds + ' um ' + ts + ' Uhr');
  lines.push('Gesamtscore:  ' + score + ' von ' + TOTAL + ' Fragen richtig (' + pct + ' %)');
  lines.push('Ergebnis:     ' + passed + ' (Bestehen ab ' + PASS + '/' + TOTAL + ')');
  lines.push('');
  lines.push('──────────────────────────────────────────────────');
  lines.push('ANTWORTEN IM DETAIL');
  lines.push('──────────────────────────────────────────────────');
  lines.push('');
  for (var i = 1; i <= TOTAL; i++) {
    var a = testAnswers[i];
    lines.push((a.correct ? '[RICHTIG]' : '[FALSCH] ') + ' ' + labels[i]);
    lines.push('         Gegeben:  ' + optTexts[i][a.chosen]);
    if (!a.correct) lines.push('         Richtig:  ' + optTexts[i][correct[i]]);
    lines.push('');
  }
  lines.push('──────────────────────────────────────────────────');
  if (score === TOTAL)        lines.push('BEWERTUNG: Perfekt – alle 20 Fragen richtig. Vollständig zertifiziert.');
  else if (score >= 18)       lines.push('BEWERTUNG: Sehr gut – ' + score + '/20. Kleinigkeiten verfeinern.');
  else if (score >= PASS)     lines.push('BEWERTUNG: Bestanden – ' + score + '/20. Einzelne Module wiederholen.');
  else                        lines.push('BEWERTUNG: Nicht bestanden – ' + score + '/20. Vollständige Wiederholung empfohlen.');
  lines.push('──────────────────────────────────────────────────');
  lines.push('');
  lines.push('Automatisch generiert – Realm Germany B2B Sales Masterclass 2025.');

  var subject = encodeURIComponent('Sales Masterclass Ergebnis: ' + name);
  var body    = encodeURIComponent(lines.join('\n'));
  window.location.href = 'mailto:m.christel@realm-europe.de?subject=' + subject + '&body=' + body;

  var note = document.getElementById('mailnote');
  note.className = 'mail-note mail-ok';
  note.textContent = 'E-Mail-Client wird geöffnet …';
}

function resetTest() {
  testAnswers = {}; testLocked = {}; testAnswered = 0; testScore = 0;
  for (var i = 1; i <= TOTAL; i++) {
    var block = document.getElementById('qb' + i);
    block.querySelectorAll('.opt').forEach(function(o){ o.className = 'opt'; });
    document.getElementById('fb' + i + 'ok').className = 'fb ok';
    document.getElementById('fb' + i + 'err').className = 'fb err';
  }
  document.getElementById('scorebox').className = 'score-box';
  document.getElementById('prog-fill').style.width = '0%';
  document.getElementById('prog-text').textContent = '0 von 20 beantwortet';
  document.getElementById('prog-score-inner').textContent = '0 richtig';
  document.getElementById('mailnote').textContent = '';
  document.getElementById('missedbox').style.display = 'none';
  window.scrollTo({ top: 0, behavior: 'smooth' });
}
</script>
</body>
</html>
