<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>164 Trek Group — Train weekly. Climb together. Safely.</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,400;9..144,500;9..144,600;9..144,700;9..144,900&family=Source+Sans+3:ital,wght@0,400;0,500;0,600;1,400&display=swap" rel="stylesheet">
<style>
  :root{
    --bg:#f0e8d8;
    --card:#f7f1e3;
    --ink:#2e2a22;
    --ink-soft:#6b6353;
    --rust:#a0552c;
    --rust-deep:#8a4724;
    --olive:#7d7a55;
    --olive-soft:#8f8c66;
    --line:#ddd2bb;
    --dark:#2e2a22;
  }
  *{box-sizing:border-box;margin:0;padding:0}
  html{scroll-behavior:smooth}
  body{
    background:var(--bg);
    color:var(--ink);
    font-family:'Source Sans 3',sans-serif;
    line-height:1.6;
    -webkit-font-smoothing:antialiased;
  }
  h1,h2,h3,h4{font-family:'Fraunces',serif;font-weight:700;letter-spacing:-0.01em;line-height:1.1}
  .wrap{max-width:1120px;margin:0 auto;padding:0 28px}
  section{padding:84px 0}
  .eyebrow{font-size:.78rem;letter-spacing:.16em;text-transform:uppercase;color:var(--rust);font-weight:600;margin-bottom:14px}

  /* ---- Nav ---- */
  nav{position:sticky;top:0;z-index:50;background:rgba(240,232,216,.88);backdrop-filter:blur(10px);border-bottom:1px solid var(--line)}
  .nav-inner{max-width:1120px;margin:0 auto;padding:14px 28px;display:flex;align-items:center;justify-content:space-between;gap:20px}
  .brand{font-family:'Fraunces',serif;font-weight:900;font-size:1.15rem;display:flex;align-items:center;gap:10px;color:var(--ink);text-decoration:none}
  .brand .num{background:var(--rust);color:#fff;border-radius:6px;padding:2px 9px;font-size:.95rem}
  .nav-links{display:flex;gap:26px;align-items:center}
  .nav-links a{color:var(--ink-soft);text-decoration:none;font-size:.92rem;font-weight:500;transition:color .2s}
  .nav-links a:hover{color:var(--rust)}
  .nav-cta{background:var(--rust);color:#fff!important;padding:9px 18px;border-radius:8px;font-weight:600}
  .nav-cta:hover{background:var(--rust-deep)}
  @media(max-width:760px){.nav-links a:not(.nav-cta){display:none}}

  /* ---- Hero ---- */
  .hero{padding:120px 0 96px;position:relative;overflow:hidden}
  .hero h1{font-size:clamp(2.6rem,6vw,5rem);max-width:14ch}
  .hero .dots{position:absolute;top:130px;right:40px;display:flex;flex-direction:column;gap:14px}
  .hero .dots span{width:22px;height:22px;border-radius:50%}
  .dot-rust{background:var(--rust)}
  .dot-olive{background:var(--olive)}
  .hero p.lede{margin-top:26px;font-size:1.22rem;color:var(--ink-soft);max-width:48ch}
  .hero-actions{margin-top:38px;display:flex;gap:14px;flex-wrap:wrap}
  .btn{display:inline-flex;align-items:center;gap:9px;padding:13px 24px;border-radius:9px;font-weight:600;font-size:1rem;text-decoration:none;transition:transform .15s,background .2s}
  .btn-primary{background:var(--rust);color:#fff}
  .btn-primary:hover{background:var(--rust-deep);transform:translateY(-2px)}
  .btn-ghost{border:1.5px solid var(--line);color:var(--ink)}
  .btn-ghost:hover{border-color:var(--rust);color:var(--rust)}

  /* ---- Cards / grids ---- */
  .grid-2{display:grid;grid-template-columns:1fr 1fr;gap:22px}
  .grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:22px}
  @media(max-width:760px){.grid-2,.grid-3{grid-template-columns:1fr}}
  .card{background:var(--card);border:1px solid var(--line);padding:30px 32px;border-radius:2px}
  .card.accent{border-left:5px solid var(--rust)}
  .card h3{font-size:1.45rem;margin-bottom:10px}
  .card p{color:var(--ink-soft)}

  .section-head{margin-bottom:44px}
  .section-head h2{font-size:clamp(2rem,4vw,2.9rem)}

  /* ---- Weekly training icons row ---- */
  .train-row{display:grid;grid-template-columns:repeat(3,1fr);gap:22px;margin-bottom:22px}
  @media(max-width:760px){.train-row{grid-template-columns:1fr}}
  .train-card{background:var(--card);border:1px solid var(--line);padding:26px 28px;display:flex;align-items:center;gap:18px}
  .train-card .ic{flex:0 0 auto;width:54px;height:54px;color:var(--rust)}
  .train-card h4{font-size:1.25rem}
  .train-card span{color:var(--ink-soft);font-size:.96rem}
  .note{font-style:italic;color:var(--ink-soft);margin:6px 0 40px}

  /* ---- Commitment tiers ---- */
  .tiers{display:grid;grid-template-columns:repeat(3,1fr);gap:22px}
  @media(max-width:860px){.tiers{grid-template-columns:1fr}}
  .tier{background:var(--card);border:1px solid var(--line)}
  .tier .top{padding:14px 20px;display:flex;justify-content:space-between;align-items:baseline;color:#fff}
  .tier .top b{font-family:'Fraunces',serif;font-size:1.2rem}
  .tier .top em{font-style:normal;font-size:.82rem;opacity:.85;margin-left:6px}
  .tier .top .hrs{font-weight:700;font-size:.92rem}
  .tier.light .top{background:var(--rust)}
  .tier.standard .top{background:var(--olive)}
  .tier.heavy .top{background:var(--dark)}
  .tier ul{list-style:none;padding:20px 22px}
  .tier li{position:relative;padding-left:18px;margin-bottom:12px;color:var(--ink-soft);font-size:.96rem}
  .tier li:before{content:"";position:absolute;left:0;top:9px;width:6px;height:6px;border-radius:50%;background:var(--rust)}

  /* ---- Candidate lists ---- */
  .lists{display:grid;grid-template-columns:1fr 1fr;gap:32px}
  @media(max-width:760px){.lists{grid-template-columns:1fr}}
  .list-block h3{font-size:1.35rem;margin-bottom:6px}
  .list-block .sub{color:var(--ink-soft);margin-bottom:18px;font-size:.95rem}
  .peak{background:var(--card);border:1px solid var(--line);border-left:4px solid var(--rust);padding:16px 20px;margin-bottom:12px}
  .peak .pk-name{font-family:'Fraunces',serif;font-weight:600;font-size:1.08rem}
  .peak .pk-meta{color:var(--ink-soft);font-size:.9rem;margin-top:2px}
  .peak .pk-desc{color:var(--ink-soft);font-size:.9rem;font-style:italic;margin-top:5px}
  .list-b .peak{border-left-color:var(--olive)}

  /* ---- Calendar ---- */
  #calendar{background:var(--card);border-top:1px solid var(--line);border-bottom:1px solid var(--line)}
  .cal-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:20px}
  @media(max-width:860px){.cal-grid{grid-template-columns:1fr 1fr}}
  @media(max-width:520px){.cal-grid{grid-template-columns:1fr}}
  .cal-card{background:var(--bg);border:1px solid var(--line);padding:24px;position:relative;overflow:hidden}
  .cal-card .when{font-family:'Fraunces',serif;font-weight:700;font-size:1.6rem;color:var(--rust)}
  .cal-card .order{font-size:.72rem;letter-spacing:.14em;text-transform:uppercase;color:var(--olive);font-weight:600;margin-bottom:10px}
  .cal-card h4{font-size:1.18rem;margin:8px 0 3px}
  .cal-card .loc{color:var(--ink-soft);font-size:.92rem}
  .cal-card .tba{display:inline-block;margin-top:12px;font-size:.74rem;letter-spacing:.1em;text-transform:uppercase;background:var(--line);color:var(--ink-soft);padding:3px 10px;border-radius:20px;font-weight:600}

  /* ---- Travel windows table ---- */
  .legend{display:flex;gap:22px;flex-wrap:wrap;margin-bottom:24px;font-size:.86rem;color:var(--ink-soft)}
  .legend span{display:inline-flex;align-items:center;gap:7px}
  .swatch{width:14px;height:14px;border-radius:3px;display:inline-block}
  .sw-prime{background:var(--rust)}
  .sw-shoulder{background:#d9b48a}
  .sw-avoid{background:#e3dcc9;border:1px solid var(--line)}
  .tw-wrap{overflow-x:auto}
  table.tw{width:100%;border-collapse:collapse;min-width:680px;font-size:.86rem}
  table.tw th,table.tw td{padding:8px 4px;text-align:center}
  table.tw thead th{color:var(--ink-soft);font-weight:600;font-size:.8rem}
  table.tw td.name{text-align:left;white-space:nowrap;padding-right:16px}
  table.tw td.name b{font-family:'Fraunces',serif;font-weight:600;font-size:.98rem;display:block}
  table.tw td.name small{color:var(--ink-soft)}
  table.tw .cell{height:22px;border-radius:3px;margin:2px 1px}
  .grp-row td{padding-top:18px;text-transform:uppercase;letter-spacing:.12em;font-size:.74rem;color:var(--rust);font-weight:700;text-align:left}

  /* ---- Pricing ---- */
  #pricing{background:var(--dark);color:#f3ecdc}
  #pricing .eyebrow{color:#d9a06b}
  #pricing h2{color:#fff}
  #pricing .intro{color:#cfc6b2;max-width:60ch;margin-bottom:14px}
  .price-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:22px;margin-top:36px}
  @media(max-width:860px){.price-grid{grid-template-columns:1fr}}
  .price-card{background:#383228;border:1px solid #4a4234;border-radius:4px;padding:28px;display:flex;flex-direction:column}
  .price-card h4{color:#fff;font-size:1.3rem;line-height:1.2}
  .price-card .incl{color:#bcb29c;font-size:.9rem;margin:8px 0 22px}
  .tier-list{list-style:none}
  .tier-list li{display:flex;justify-content:space-between;align-items:baseline;padding:11px 0;border-bottom:1px solid #4a4234}
  .tier-list li:last-child{border-bottom:none}
  .tier-list .grp{color:#cfc6b2;font-size:.92rem}
  .tier-list .amt{font-family:'Fraunces',serif;font-weight:600;color:#f3ecdc;font-size:1.12rem}
  .tier-list li:first-child .amt{color:#e8a866}
  .price-foot{color:#9c937e;font-size:.82rem;margin-top:30px;max-width:70ch}

  /* ---- Coaching / baseline ---- */
  .bench{background:var(--rust);color:#fff;border-radius:2px;padding:40px 34px;display:flex;flex-direction:column;justify-content:center;align-items:center;text-align:center}
  .bench .lab{font-size:.85rem;letter-spacing:.1em;opacity:.85;margin-bottom:10px}
  .bench .big{font-family:'Fraunces',serif;font-weight:700;font-size:1.7rem;line-height:1.2}
  .bench .yic{width:70px;height:70px;margin-bottom:20px}
  .baseline-list{columns:2;column-gap:34px}
  @media(max-width:620px){.baseline-list{columns:1}}
  .baseline-list li{break-inside:avoid;margin-bottom:14px;padding-left:18px;position:relative;color:var(--ink-soft);font-size:.96rem}
  .baseline-list li:before{content:"";position:absolute;left:0;top:9px;width:6px;height:6px;border-radius:50%;background:var(--olive)}

  /* ---- Need back steps ---- */
  .steps{counter-reset:step}
  .step{display:flex;gap:20px;padding:22px 0;border-bottom:1px solid var(--line)}
  .step:last-child{border-bottom:none}
  .step .n{counter-increment:step;flex:0 0 auto;width:40px;height:40px;border-radius:50%;background:var(--rust);color:#fff;font-family:'Fraunces',serif;font-weight:700;display:flex;align-items:center;justify-content:center}
  .step .n:before{content:counter(step)}
  .step h4{font-size:1.2rem;margin-bottom:4px}
  .step p,.step ul{color:var(--ink-soft);font-size:.95rem}
  .step ul{list-style:none;margin-top:6px}
  .step ul li{padding-left:16px;position:relative;margin-bottom:4px}
  .step ul li:before{content:"–";position:absolute;left:0;color:var(--rust)}

  /* ---- CTA / contact ---- */
  #signup{text-align:center}
  #signup h2{font-size:clamp(2rem,5vw,3.2rem);margin-bottom:18px}
  #signup p{color:var(--ink-soft);max-width:50ch;margin:0 auto 30px;font-size:1.1rem}
  .wa-btn{display:inline-flex;align-items:center;gap:12px;background:#25d366;color:#fff;text-decoration:none;font-weight:700;font-size:1.15rem;padding:16px 30px;border-radius:12px;transition:transform .15s,filter .2s}
  .wa-btn:hover{transform:translateY(-2px);filter:brightness(.96)}
  .wa-btn svg{width:26px;height:26px}
  .wa-num{margin-top:16px;color:var(--ink-soft);font-size:1rem}
  .dates-row{display:flex;gap:22px;justify-content:center;flex-wrap:wrap;margin-top:40px}
  .date-box{background:var(--card);border:1px solid var(--line);border-left:4px solid var(--rust);padding:18px 26px;min-width:200px;text-align:left}
  .date-box .t{font-family:'Fraunces',serif;font-weight:700;font-size:1.1rem;margin-bottom:4px}
  .date-box .d{color:var(--ink-soft)}

  footer{background:var(--dark);color:#cfc6b2;text-align:center;padding:40px 20px;font-size:.9rem}
  footer .brand{justify-content:center;color:#fff;margin-bottom:10px}
  footer a{color:#e8a866;text-decoration:none}

  /* reveal */
  .reveal{opacity:0;transform:translateY(20px);transition:opacity .7s ease,transform .7s ease}
  .reveal.in{opacity:1;transform:none}
</style>
</head>
<body>

<nav>
  <div class="nav-inner">
    <a href="#top" class="brand"><span class="num">164</span> Trek Group</a>
    <div class="nav-links">
      <a href="#principles">Principles</a>
      <a href="#training">Training</a>
      <a href="#peaks">Peaks</a>
      <a href="#calendar">Calendar</a>
      <a href="#pricing">Pricing</a>
      <a href="#signup" class="nav-cta">Sign up</a>
    </div>
  </div>
</nav>

<header class="hero" id="top">
  <div class="wrap">
    <div class="dots">
      <span class="dot-rust"></span>
      <span class="dot-olive"></span>
    </div>
    <div class="eyebrow">164 Trek Group</div>
    <h1>Train weekly. Climb together. Safely.</h1>
    <p class="lede">A walking-trails-only trekking group. We build the fitness to finish comfortably, start with one mountain, and keep each other accountable along the way.</p>
    <div class="hero-actions">
      <a href="#signup" class="btn btn-primary">Sign up on WhatsApp</a>
      <a href="#calendar" class="btn btn-ghost">See the calendar</a>
    </div>
  </div>
</header>

<!-- PRINCIPLES -->
<section id="principles">
  <div class="wrap">
    <div class="section-head reveal"><h2>Design principles</h2></div>
    <div class="grid-2">
      <div class="card accent reveal"><h3>No falling risk</h3><p>Walking trails only. Altitude, scree, weather, mud are fine. Ropes, exposed ridges, glaciers are out.</p></div>
      <div class="card accent reveal"><h3>Start small</h3><p>One mountain first, then the group decides what's next.</p></div>
      <div class="card accent reveal"><h3>Prepared, not rushed</h3><p>We build the fitness to finish comfortably and enjoy the whole way up.</p></div>
      <div class="card accent reveal"><h3>Mutual accountability</h3><p>We encourage each other on training, recovery, diet.</p></div>
    </div>
  </div>
</section>

<!-- TRAINING -->
<section id="training" style="background:var(--card);border-top:1px solid var(--line);border-bottom:1px solid var(--line)">
  <div class="wrap">
    <div class="section-head reveal"><h2>Weekly training</h2></div>
    <div class="train-row">
      <div class="train-card reveal">
        <svg class="ic" viewBox="0 0 64 40" fill="none" stroke="currentColor" stroke-width="5" stroke-linecap="round">
          <path d="M4 10c6-7 12 7 18 0s12 7 18 0 12 7 18 0"/><path d="M4 22c6-7 12 7 18 0s12 7 18 0 12 7 18 0"/><path d="M4 34c6-7 12 7 18 0s12 7 18 0 12 7 18 0"/>
        </svg>
        <div><h4>River Valley</h4><span>long runs, weighted-pack walks</span></div>
      </div>
      <div class="train-card reveal">
        <svg class="ic" viewBox="0 0 64 64" fill="currentColor">
          <rect x="28" y="2" width="8" height="8" rx="2"/><circle cx="32" cy="38" r="22" fill="none" stroke="currentColor" stroke-width="5"/><rect x="30" y="22" width="4" height="18" rx="2"/>
        </svg>
        <div><h4>Stadium (Kallang)</h4><span>stairs, steady endurance sets</span></div>
      </div>
      <div class="train-card reveal">
        <svg class="ic" viewBox="0 0 64 64" fill="currentColor">
          <path d="M6 54 L26 18 L36 36 L44 24 L58 54 Z"/><path d="M22 26 l4 -7 l4 7 l-4 5 z" fill="var(--card)"/>
        </svg>
        <div><h4>Bukit Timah</h4><span>vertical repeats with pack</span></div>
      </div>
    </div>
    <p class="note reveal">Grouped by fitness. On the mountain, multiple guides so everyone has company at a comfortable pace.</p>

    <h3 style="font-size:1.6rem;margin-bottom:24px" class="reveal">What a weekly commitment looks like</h3>
    <div class="tiers">
      <div class="tier light reveal">
        <div class="top"><span><b>Light</b><em>entry</em></span><span class="hrs">~3 hr/wk</span></div>
        <ul>
          <li>1 group session + solo MWF</li>
          <li>Solo: easy jog every morning or evening, no pack</li>
          <li>Sat group: Bukit Timah, 2 repeats with 5kg pack (~2 hr)</li>
        </ul>
      </div>
      <div class="tier standard reveal">
        <div class="top"><span><b>Standard</b></span><span class="hrs">~5–6 hr/wk</span></div>
        <ul>
          <li>2 group sessions + 1 solo</li>
          <li>Tue PM: Kallang stadium, stairs and endurance (~1 hr)</li>
          <li>Sat AM: Bukit Timah, 3–4 repeats with 8kg pack (~2.5 hr)</li>
          <li>Sun or solo: long PCN walk/run, 90 min</li>
        </ul>
      </div>
      <div class="tier heavy reveal">
        <div class="top"><span><b>Heavy</b><em>pre-climb block</em></span><span class="hrs">~8–10 hr/wk</span></div>
        <ul>
          <li>3 group + 2 solo</li>
          <li>Adds a second hill day, longer pack carries, back-to-back weekends</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<!-- PEAKS -->
<section id="peaks">
  <div class="wrap">
    <div class="section-head reveal">
      <h2>Ten candidates, two lists</h2>
      <p style="color:var(--ink-soft);margin-top:10px;max-width:60ch">We start with one from List A. Once it's done, the group picks one from List B.</p>
    </div>
    <div class="lists">
      <div class="list-block list-a reveal">
        <h3>List A — easy access</h3>
        <p class="sub">Start here.</p>
        <div class="peak"><span class="pk-name">Kinabalu, Malaysia</span><div class="pk-meta">4,095 m · Standard 2 days</div><div class="pk-desc">We summit comfortably in a guided day group.</div></div>
        <div class="peak"><span class="pk-name">Rinjani, Indonesia</span><div class="pk-meta">3,726 m · Standard 3 days</div><div class="pk-desc">We plan a well-paced 2–3 day itinerary.</div></div>
        <div class="peak"><span class="pk-name">Annapurna Circuit, Nepal</span><div class="pk-meta">5,416 m · Standard 15–20 days</div><div class="pk-desc">We follow a safe, steady schedule.</div></div>
      </div>
      <div class="list-block list-b reveal">
        <h3>List B — longer haul</h3>
        <p class="sub">Next round.</p>
        <div class="peak"><span class="pk-name">Tongariro Northern Circuit, NZ</span><div class="pk-meta">43 km · Std 3–4 days</div></div>
        <div class="peak"><span class="pk-name">Overland Track, Tasmania</span><div class="pk-meta">65 km · Std 6–8 days</div></div>
        <div class="peak"><span class="pk-name">Goecha La, Sikkim India</span><div class="pk-meta">4,940 m · Std 10–11 days</div></div>
        <div class="peak"><span class="pk-name">Tour du Mont Blanc</span><div class="pk-meta">170 km · Std 10–12 days</div></div>
        <div class="peak"><span class="pk-name">Kilimanjaro, Tanzania</span><div class="pk-meta">5,895 m · Std 7–9 days</div></div>
        <div class="peak"><span class="pk-name">Toubkal, Morocco</span><div class="pk-meta">4,167 m · Std 2–3 days</div></div>
        <div class="peak"><span class="pk-name">Huayhuash Circuit, Peru</span><div class="pk-meta">130 km · Std 8–12 days</div></div>
      </div>
    </div>
  </div>
</section>

<!-- TRAVEL WINDOWS -->
<section id="windows" style="background:var(--card);border-top:1px solid var(--line);border-bottom:1px solid var(--line)">
  <div class="wrap">
    <div class="section-head reveal">
      <h2>Best travel windows</h2>
      <p style="color:var(--ink-soft);margin-top:10px">When each climb is comfortable to do over the year.</p>
    </div>
    <div class="legend reveal">
      <span><i class="swatch sw-prime"></i> Prime — best months</span>
      <span><i class="swatch sw-shoulder"></i> Shoulder — workable</span>
      <span><i class="swatch sw-avoid"></i> Avoid — wet / closed</span>
    </div>
    <div class="tw-wrap reveal">
      <table class="tw" id="twtable">
        <thead><tr><th class="name"></th>
          <th>J</th><th>F</th><th>M</th><th>A</th><th>M</th><th>J</th><th>J</th><th>A</th><th>S</th><th>O</th><th>N</th><th>D</th>
          <th style="text-align:left;padding-left:14px">Best window</th></tr></thead>
        <tbody id="twbody"></tbody>
      </table>
    </div>
  </div>
</section>

<!-- CALENDAR -->
<section id="calendar">
  <div class="wrap">
    <div class="section-head reveal">
      <h2>Our calendar</h2>
      <p style="color:var(--ink-soft);margin-top:10px;max-width:60ch">Four climbs mapped across the year. Exact dates are still being set — they're marked TBA for now.</p>
    </div>
    <div class="cal-grid">
      <div class="cal-card reveal"><div class="order">First climb · List A</div><div class="when">July</div><h4>Rinjani</h4><div class="loc">Indonesia · 3,726 m</div><span class="tba">Date TBA</span></div>
      <div class="cal-card reveal"><div class="order">List B</div><div class="when">October</div><h4>Goecha La</h4><div class="loc">Sikkim, India · 4,940 m</div><span class="tba">Date TBA</span></div>
      <div class="cal-card reveal"><div class="order">List B</div><div class="when">Late Nov</div><h4>NZ or Tasmania</h4><div class="loc">Tongariro 43 km / Overland 65 km</div><span class="tba">Date TBA</span></div>
      <div class="cal-card reveal"><div class="order">List B</div><div class="when">Late Jan</div><h4>Kilimanjaro</h4><div class="loc">Tanzania · 5,895 m</div><span class="tba">Date TBA</span></div>
    </div>
  </div>
</section>

<!-- PRICING -->
<section id="pricing">
  <div class="wrap">
    <div class="eyebrow reveal">Pricing · per pax</div>
    <h2 class="reveal">Rinjani packages</h2>
    <p class="intro reveal">Our first climb. Three itineraries, priced per person across group-size tiers — the larger the group, the lower the per-pax rate.</p>
    <div class="price-grid">
      <div class="price-card reveal">
        <h4>2D / 1N</h4>
        <div class="incl">Crater Rim</div>
        <ul class="tier-list">
          <li><span class="grp">Tier 1</span><span class="amt">$420</span></li>
          <li><span class="grp">Tier 2</span><span class="amt">$270</span></li>
          <li><span class="grp">Tier 3</span><span class="amt">$220</span></li>
          <li><span class="grp">Tier 4</span><span class="amt">$180</span></li>
          <li><span class="grp">Tier 5</span><span class="amt">$160</span></li>
        </ul>
      </div>
      <div class="price-card reveal">
        <h4>3D / 2N</h4>
        <div class="incl">+ Summit, Lake, Hot Spring</div>
        <ul class="tier-list">
          <li><span class="grp">Tier 1</span><span class="amt">$520</span></li>
          <li><span class="grp">Tier 2</span><span class="amt">$320</span></li>
          <li><span class="grp">Tier 3</span><span class="amt">$280</span></li>
          <li><span class="grp">Tier 4</span><span class="amt">$240</span></li>
          <li><span class="grp">Tier 5</span><span class="amt">$210</span></li>
        </ul>
      </div>
      <div class="price-card reveal">
        <h4>4D / 3N</h4>
        <div class="incl">+ Summit, Lake, Hot Spring</div>
        <ul class="tier-list">
          <li><span class="grp">Tier 1</span><span class="amt">$670</span></li>
          <li><span class="grp">Tier 2</span><span class="amt">$420</span></li>
          <li><span class="grp">Tier 3</span><span class="amt">$370</span></li>
          <li><span class="grp">Tier 4</span><span class="amt">$320</span></li>
          <li><span class="grp">Tier 5</span><span class="amt">$280</span></li>
        </ul>
      </div>
    </div>
    <p class="price-foot reveal">Prices are per person and decrease with larger group sizes (Tier 1 = smallest group). Message us on WhatsApp for the exact rate for your group.</p>
  </div>
</section>

<!-- COACHING + BASELINE -->
<section id="coaching">
  <div class="wrap">
    <div class="section-head reveal"><h2>How we coach each other</h2></div>
    <div class="grid-2" style="margin-bottom:22px">
      <div style="display:flex;flex-direction:column;gap:22px">
        <div class="card accent reveal"><h3>Progress check-ins, weekly</h3><p>How training is going, how recovery feels, comfortable Bukit Timah round trips.</p></div>
        <div class="card accent reveal"><h3>Light diet check-ins</h3><p>No preaching.</p></div>
      </div>
      <div class="bench reveal">
        <svg class="yic" viewBox="0 0 100 100" fill="none" stroke="#fff" stroke-width="5">
          <path d="M50 12 L86 74 L14 74 Z"/>
          <path d="M50 44 c-7 6 -7 16 0 22 c7 -6 7 -16 0 -22 Z" fill="#fff" stroke="none"/>
          <path d="M50 50 c-9 -2 -16 4 -16 12 c9 2 16 -4 16 -12 Z" fill="#fff" stroke="none"/>
          <path d="M50 50 c9 -2 16 4 16 12 c-9 2 -16 -4 -16 -12 Z" fill="#fff" stroke="none"/>
        </svg>
        <div class="lab">Fitness benchmark</div>
        <div class="big">Full Ashtanga primary series at the summit</div>
      </div>
    </div>
  </div>
</section>

<!-- BASELINE -->
<section id="baseline" style="background:var(--card);border-top:1px solid var(--line);border-bottom:1px solid var(--line)">
  <div class="wrap">
    <div class="section-head reveal">
      <h2>Baseline</h2>
      <p style="color:var(--ink-soft);margin-top:10px">For grouping, not gatekeeping. About finishing safely, not racing.</p>
    </div>
    <ul class="baseline-list reveal">
      <li>Resting HR (e.g., 52)</li>
      <li>Bukit Timah round trip, no pack (e.g., comfortable in 65 min)</li>
      <li>100 floors at Pinnacle@Duxton with 5kg pack (how it felt)</li>
      <li>How far you can walk/run without strain in 12 minutes (e.g., 2.5 km)</li>
      <li>Longest trek in last 2 years (e.g., 4-day hike in Nepal, 2024)</li>
      <li>Weekly cardio hours (e.g., 4 hr)</li>
      <li>Altitude experience above 3,000 m (e.g., once, 4,200 m)</li>
      <li>Injuries (e.g., minor knee strain, managed)</li>
    </ul>
  </div>
</section>

<!-- WHAT WE NEED BACK -->
<section id="needback">
  <div class="wrap">
    <div class="section-head reveal"><h2>What we need back</h2></div>
    <div class="steps reveal">
      <div class="step">
        <div class="n"></div>
        <div>
          <h4>Pick one from List A and one from List B</h4>
          <p>We start with List A. List B is the next round.</p>
          <ul>
            <li><b>List A:</b> Kinabalu (4,095 m), Rinjani (3,726 m), Annapurna Circuit (5,416 m)</li>
            <li><b>List B:</b> Tongariro NZ (43 km), Overland Tasmania (65 km), Goecha La India (4,940 m), Tour du Mont Blanc (170 km), Kilimanjaro Tanzania (5,895 m), Toubkal Morocco (4,167 m), Huayhuash Peru (130 km)</li>
          </ul>
        </div>
      </div>
      <div class="step"><div class="n"></div><div><h4>Date windows over the next 12 months</h4></div></div>
      <div class="step"><div class="n"></div><div><h4>Training commitment</h4><p>Yes / probably / hard no</p></div></div>
      <div class="step">
        <div class="n"></div>
        <div><h4>Baseline</h4>
          <ul>
            <li>Resting HR · Bukit Timah round trip (no pack) · 100 floors at Pinnacle@Duxton with 5kg pack</li>
            <li>12-min walk/run distance · longest trek in last 2 years · weekly cardio hours</li>
            <li>Altitude experience above 3,000 m · injuries</li>
          </ul>
        </div>
      </div>
      <div class="step"><div class="n"></div><div><h4>Cost ceiling</h4></div></div>
    </div>
  </div>
</section>

<!-- SIGNUP -->
<section id="signup">
  <div class="wrap">
    <div class="eyebrow reveal" style="text-align:center">Train weekly. Climb together. Safely.</div>
    <h2 class="reveal">Sign up to join</h2>
    <p class="reveal">Message us on WhatsApp to join, ask about the trial session, or send your baseline. Easy.</p>
    <a class="wa-btn reveal" href="https://wa.me/qr/5MDC44IBSXFPN1?text=Hi!%20I'd%20like%20to%20join%20the%20164%20Trek%20Group." target="_blank" rel="noopener">
      <svg viewBox="0 0 32 32" fill="currentColor"><path d="M16 .5C7.4.5.5 7.4.5 16c0 2.8.7 5.4 2 7.7L.5 31.5l8-2.1c2.2 1.2 4.8 1.9 7.5 1.9 8.6 0 15.5-6.9 15.5-15.5S24.6.5 16 .5zm0 28.3c-2.4 0-4.7-.7-6.7-1.9l-.5-.3-4.7 1.2 1.3-4.6-.3-.5a12.8 12.8 0 01-2-6.9C3.1 8.9 8.9 3.1 16 3.1S28.9 8.9 28.9 16 23.1 28.8 16 28.8zm7.1-9.6c-.4-.2-2.3-1.1-2.7-1.3-.4-.1-.6-.2-.9.2-.3.4-1 1.3-1.2 1.5-.2.2-.4.3-.8.1-.4-.2-1.6-.6-3.1-1.9-1.1-1-1.9-2.3-2.1-2.7-.2-.4 0-.6.2-.8.2-.2.4-.4.6-.7.2-.2.3-.4.4-.7.1-.2.1-.5 0-.7-.1-.2-.9-2.2-1.3-3-.3-.8-.7-.7-.9-.7h-.8c-.3 0-.7.1-1 .5-.4.4-1.4 1.3-1.4 3.3s1.4 3.8 1.6 4.1c.2.3 2.8 4.3 6.8 6 .9.4 1.7.6 2.3.8.9.3 1.8.2 2.5.1.8-.1 2.3-.9 2.6-1.9.3-.9.3-1.7.2-1.9-.1-.2-.4-.3-.8-.5z"/></svg>
      Sign up on WhatsApp
    </a>
    <div class="wa-num reveal">Message us</div>
    <div class="dates-row">
      <div class="date-box reveal"><div class="t">Trial session</div><div class="d">Date: TBA</div></div>
      <div class="date-box reveal"><div class="t">Reply by</div><div class="d">Date: TBA</div></div>
    </div>
  </div>
</section>

<footer>
  <div class="brand"><span class="num">164</span> Trek Group</div>
  <div>Train weekly. Climb together. Safely.</div>
  <div style="margin-top:8px">WhatsApp <a href="https://wa.me/qr/5MDC44IBSXFPN1" target="_blank" rel="noopener">Message us</a></div>
</footer>

<script>
// Travel windows data: 0=avoid,1=shoulder,2=prime  (Jan..Dec)
const windows=[
  {grp:"List A — start here"},
  {name:"Kinabalu",loc:"Malaysia · 4,095 m",best:"Feb–Apr",m:[1,2,2,2,1,1,1,1,1,0,0,1]},
  {name:"Rinjani",loc:"Indonesia · 3,726 m",best:"May–Oct",m:[0,0,1,1,2,2,2,2,2,2,1,0]},
  {name:"Annapurna Circuit",loc:"Nepal · 5,416 m",best:"Oct–Nov, Mar–Apr",m:[0,1,2,2,1,0,0,0,1,2,2,1]},
  {grp:"List B — next round"},
  {name:"Tongariro Circuit",loc:"New Zealand · 43 km",best:"Dec–Mar",m:[2,2,2,1,0,0,0,0,1,1,1,2]},
  {name:"Overland Track",loc:"Tasmania · 65 km",best:"Dec–Mar",m:[2,2,2,1,0,0,0,0,1,1,1,2]},
  {name:"Goecha La",loc:"Sikkim · 4,940 m",best:"Mar–May, Oct–Nov",m:[0,1,2,2,2,0,0,0,1,2,2,1]},
  {name:"Tour du Mont Blanc",loc:"Alps · 170 km",best:"Jul–Sep",m:[0,0,0,0,1,1,2,2,2,1,0,0]},
  {name:"Kilimanjaro",loc:"Tanzania · 5,895 m",best:"Jan–Feb, Jun–Oct",m:[2,2,1,0,0,2,2,2,2,2,1,1]},
  {name:"Toubkal",loc:"Morocco · 4,167 m",best:"Apr–Jun, Sep–Oct",m:[0,1,1,2,2,2,1,1,2,2,1,0]},
  {name:"Huayhuash Circuit",loc:"Peru · 130 km",best:"May–Sep",m:[0,0,1,1,2,2,2,2,2,1,0,0]}
];
const colors={0:"var(--sw-avoid,#e3dcc9)",1:"#d9b48a",2:"var(--rust)"};
const body=document.getElementById('twbody');
windows.forEach(r=>{
  const tr=document.createElement('tr');
  if(r.grp){tr.className='grp-row';tr.innerHTML=`<td colspan="14">${r.grp}</td>`;body.appendChild(tr);return;}
  let cells=`<td class="name"><b>${r.name}</b><small>${r.loc}</small></td>`;
  r.m.forEach(v=>{const c=v===2?'var(--rust)':v===1?'#d9b48a':'#e3dcc9';const b=v===0?'border:1px solid var(--line);':'';cells+=`<td><div class="cell" style="background:${c};${b}"></div></td>`;});
  cells+=`<td style="text-align:left;padding-left:14px;color:var(--ink-soft);white-space:nowrap">${r.best}</td>`;
  tr.innerHTML=cells;body.appendChild(tr);
});

// scroll reveal
const io=new IntersectionObserver((es)=>{es.forEach(e=>{if(e.isIntersecting){e.target.classList.add('in');io.unobserve(e.target);}})},{threshold:.12});
document.querySelectorAll('.reveal').forEach((el,i)=>{el.style.transitionDelay=(i%4*0.06)+'s';io.observe(el);});
</script>
</body>
</html>
