<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Muhammad Qasim Academy – Free System Design Mastery</title>
<link href="https://fonts.googleapis.com/css2?family=Sora:wght@400;600;700;800&family=Inter:wght@400;500;600&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet"/>
<style>
  :root {
    --navy:      #080D1A;
    --navy2:     #0E1629;
    --navy3:     #14203A;
    --gold:      #F5B800;
    --gold-dim:  #C49200;
    --cyan:      #38BDF8;
    --white:     #F0F4FF;
    --muted:     #7A8AAA;
    --card-bg:   #111827;
    --border:    rgba(245,184,0,.18);
    --radius:    14px;
  }
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
  html { scroll-behavior: smooth; }
  body {
    background: var(--navy);
    color: var(--white);
    font-family: 'Inter', sans-serif;
    font-size: 16px;
    line-height: 1.7;
    overflow-x: hidden;
  }

  /* ─── NAV ─── */
  nav {
    position: sticky; top: 0; z-index: 100;
    background: rgba(8,13,26,.85);
    backdrop-filter: blur(12px);
    border-bottom: 1px solid var(--border);
    padding: 0 clamp(1rem,5vw,4rem);
    display: flex; align-items: center; justify-content: space-between;
    height: 64px;
  }
  .logo { font-family:'Sora',sans-serif; font-weight:800; font-size:1.05rem; color:var(--gold); letter-spacing:-.3px; }
  .logo span { color: var(--white); }
  .nav-links { display:flex; gap:2rem; list-style:none; }
  .nav-links a { color:var(--muted); text-decoration:none; font-size:.9rem; font-weight:500; transition:color .2s; }
  .nav-links a:hover { color:var(--gold); }
  .nav-cta {
    background: var(--gold); color: var(--navy); font-weight:700; font-size:.85rem;
    padding:.5rem 1.2rem; border-radius:8px; text-decoration:none; transition:opacity .2s;
  }
  .nav-cta:hover { opacity:.88; }

  /* ─── HERO ─── */
  .hero {
    min-height: 92vh;
    display: flex; flex-direction: column; align-items: center; justify-content: center;
    text-align: center;
    padding: 6rem clamp(1rem,6vw,4rem) 4rem;
    position: relative; overflow: hidden;
  }
  .hero::before {
    content:'';
    position: absolute; inset: 0;
    background: radial-gradient(ellipse 80% 60% at 50% 0%, rgba(245,184,0,.12) 0%, transparent 70%),
                radial-gradient(ellipse 60% 40% at 80% 80%, rgba(56,189,248,.07) 0%, transparent 60%);
    pointer-events: none;
  }
  .free-pill {
    display: inline-flex; align-items: center; gap:.5rem;
    background: rgba(245,184,0,.12); border:1px solid var(--gold);
    color: var(--gold); font-size:.8rem; font-weight:700; letter-spacing:.08em; text-transform:uppercase;
    padding:.4rem 1rem; border-radius:99px; margin-bottom:1.8rem;
    animation: pulse-ring 2.4s ease-in-out infinite;
  }
  @keyframes pulse-ring {
    0%,100% { box-shadow: 0 0 0 0 rgba(245,184,0,.4); }
    50%      { box-shadow: 0 0 0 10px rgba(245,184,0,0); }
  }
  .hero h1 {
    font-family:'Sora',sans-serif; font-weight:800;
    font-size: clamp(2.2rem,6vw,4.4rem); line-height:1.12;
    letter-spacing:-1.5px; max-width:820px;
  }
  .hero h1 .accent { color: var(--gold); }
  .hero-sub {
    color: var(--muted); font-size:clamp(1rem,2vw,1.2rem);
    max-width:600px; margin:1.4rem auto 2.4rem;
  }
  .hero-actions { display:flex; gap:1rem; flex-wrap:wrap; justify-content:center; }
  .btn-primary {
    background: var(--gold); color: var(--navy);
    font-weight:700; font-size:1rem; padding:.85rem 2rem;
    border-radius:10px; text-decoration:none; transition:transform .15s, opacity .15s;
  }
  .btn-primary:hover { transform:translateY(-2px); opacity:.9; }
  .btn-secondary {
    background: transparent; color: var(--white);
    font-weight:600; font-size:1rem; padding:.85rem 2rem;
    border-radius:10px; text-decoration:none;
    border:1.5px solid rgba(255,255,255,.2); transition:border-color .2s, background .2s;
  }
  .btn-secondary:hover { border-color:var(--gold); background:rgba(245,184,0,.06); }

  .hero-stats {
    display:flex; gap:3rem; justify-content:center; flex-wrap:wrap;
    margin-top:4rem; padding-top:2rem; border-top:1px solid var(--border);
  }
  .stat-val { font-family:'Sora',sans-serif; font-weight:800; font-size:2rem; color:var(--gold); }
  .stat-lbl { color:var(--muted); font-size:.85rem; margin-top:.2rem; }

  /* ─── SECTIONS ─── */
  section { padding: 6rem clamp(1rem,6vw,4rem); }
  .section-label {
    font-size:.75rem; font-weight:700; letter-spacing:.15em; text-transform:uppercase;
    color:var(--gold); margin-bottom:.8rem;
  }
  .section-title {
    font-family:'Sora',sans-serif; font-weight:800;
    font-size:clamp(1.8rem,4vw,2.8rem); line-height:1.2;
    letter-spacing:-.5px; max-width:640px;
  }
  .section-sub { color:var(--muted); margin-top:.8rem; max-width:560px; }
  .center { text-align:center; margin:0 auto; }
  .center .section-title, .center .section-sub { margin:0 auto; }

  /* ─── WHY FREE ─── */
  .why-grid {
    display:grid; grid-template-columns:repeat(auto-fit,minmax(260px,1fr));
    gap:1.5rem; margin-top:3.5rem;
  }
  .why-card {
    background: var(--card-bg); border:1px solid var(--border);
    border-radius:var(--radius); padding:1.8rem;
    transition:border-color .2s, transform .2s;
  }
  .why-card:hover { border-color:var(--gold); transform:translateY(-3px); }
  .why-icon { font-size:1.8rem; margin-bottom:1rem; }
  .why-card h3 { font-family:'Sora',sans-serif; font-weight:700; font-size:1.05rem; margin-bottom:.5rem; }
  .why-card p { color:var(--muted); font-size:.9rem; }

  /* ─── CURRICULUM ─── */
  .curriculum-bg { background: var(--navy2); }
  .modules { margin-top:3rem; display:flex; flex-direction:column; gap:1rem; max-width:860px; margin-left:auto; margin-right:auto; }
  .module {
    background: var(--card-bg); border:1px solid var(--border);
    border-radius:var(--radius); overflow:hidden;
  }
  .module-header {
    display:flex; align-items:center; justify-content:space-between;
    padding:1.2rem 1.6rem; cursor:pointer;
    transition:background .2s;
    user-select:none;
  }
  .module-header:hover { background:rgba(245,184,0,.04); }
  .module-num {
    font-family:'JetBrains Mono',monospace; font-size:.75rem; font-weight:500;
    color:var(--gold-dim); margin-right:.8rem; flex-shrink:0;
  }
  .module-title { font-family:'Sora',sans-serif; font-weight:700; font-size:1rem; flex:1; }
  .module-meta { color:var(--muted); font-size:.8rem; margin-left:1rem; flex-shrink:0; }
  .module-chevron { color:var(--gold); font-size:1rem; transition:transform .3s; flex-shrink:0; margin-left:.8rem; }
  .module.open .module-chevron { transform:rotate(180deg); }
  .module-body {
    max-height:0; overflow:hidden;
    transition:max-height .4s cubic-bezier(.4,0,.2,1);
  }
  .module.open .module-body { max-height:2000px; }
  .lesson-list { padding:.4rem 1.6rem 1.4rem; list-style:none; display:flex; flex-direction:column; gap:.3rem; }
  .lesson-list li {
    display:flex; align-items:center; gap:.7rem;
    padding:.5rem .7rem; border-radius:8px; font-size:.9rem;
    transition:background .15s;
  }
  .lesson-list li:hover { background:rgba(245,184,0,.06); }
  .lesson-dot { width:6px; height:6px; border-radius:50%; background:var(--gold); flex-shrink:0; }
  .lesson-list li span { color:var(--muted); }
  .lesson-badge {
    margin-left:auto; font-size:.7rem; font-weight:700; text-transform:uppercase;
    letter-spacing:.06em; padding:.2rem .5rem; border-radius:4px;
  }
  .lb-new { background:rgba(56,189,248,.15); color:var(--cyan); }

  /* ─── TOPICS GRID ─── */
  .topics-grid {
    display:grid; grid-template-columns:repeat(auto-fill,minmax(200px,1fr));
    gap:1rem; margin-top:3rem;
  }
  .topic-chip {
    background:var(--card-bg); border:1px solid var(--border);
    border-radius:10px; padding:1rem 1.2rem;
    display:flex; align-items:center; gap:.7rem;
    font-size:.88rem; font-weight:500;
    transition:border-color .2s, transform .15s;
  }
  .topic-chip:hover { border-color:var(--gold); transform:translateY(-2px); }
  .topic-chip .ti { font-size:1.1rem; }

  /* ─── CASE STUDIES ─── */
  .cases-grid {
    display:grid; grid-template-columns:repeat(auto-fill,minmax(240px,1fr));
    gap:1.2rem; margin-top:3rem;
  }
  .case-card {
    background:var(--card-bg); border:1px solid var(--border);
    border-radius:var(--radius); padding:1.5rem;
    display:flex; align-items:flex-start; gap:1rem;
    transition:border-color .2s;
  }
  .case-card:hover { border-color:var(--cyan); }
  .case-icon { font-size:2rem; flex-shrink:0; }
  .case-card h4 { font-family:'Sora',sans-serif; font-weight:700; font-size:.95rem; }
  .case-card p { color:var(--muted); font-size:.83rem; margin-top:.3rem; }

  /* ─── HOW TO USE ─── */
  .steps { display:grid; grid-template-columns:repeat(auto-fit,minmax(220px,1fr)); gap:2rem; margin-top:3.5rem; }
  .step { text-align:center; }
  .step-circle {
    width:56px; height:56px; border-radius:50%;
    background:rgba(245,184,0,.1); border:2px solid var(--gold);
    display:flex; align-items:center; justify-content:center;
    font-family:'Sora',sans-serif; font-weight:800; font-size:1.2rem; color:var(--gold);
    margin:0 auto 1.2rem;
  }
  .step h3 { font-family:'Sora',sans-serif; font-weight:700; font-size:1rem; margin-bottom:.4rem; }
  .step p { color:var(--muted); font-size:.88rem; }

  /* ─── CTA BANNER ─── */
  .cta-banner {
    background: linear-gradient(135deg,rgba(245,184,0,.12) 0%,rgba(56,189,248,.06) 100%);
    border:1px solid var(--border); border-radius:20px;
    padding:4rem clamp(2rem,6vw,5rem); text-align:center;
    margin:0 clamp(1rem,4vw,4rem) 6rem;
  }
  .cta-banner h2 { font-family:'Sora',sans-serif; font-weight:800; font-size:clamp(1.8rem,4vw,2.6rem); letter-spacing:-.5px; }
  .cta-banner p { color:var(--muted); margin:.8rem auto 2rem; max-width:480px; }

  /* ─── FOOTER ─── */
  footer {
    background:var(--navy2); border-top:1px solid var(--border);
    padding:3rem clamp(1rem,6vw,4rem);
    display:flex; flex-direction:column; align-items:center; gap:1.5rem; text-align:center;
  }
  footer .logo { font-size:1.1rem; }
  .footer-links { display:flex; gap:2rem; flex-wrap:wrap; justify-content:center; }
  .footer-links a { color:var(--muted); font-size:.85rem; text-decoration:none; }
  .footer-links a:hover { color:var(--gold); }
  footer .copy { color:var(--muted); font-size:.82rem; }

  /* ─── SCROLLBAR ─── */
  ::-webkit-scrollbar { width:6px; }
  ::-webkit-scrollbar-track { background:var(--navy); }
  ::-webkit-scrollbar-thumb { background:var(--navy3); border-radius:3px; }

  /* ─── RESPONSIVE ─── */
  @media(max-width:640px) {
    .nav-links { display:none; }
    .hero-stats { gap:2rem; }
  }
</style>
</head>
<body>

<!-- NAV -->
<nav>
  <div class="logo">Muhammad Qasim <span>Academy</span></div>
  <ul class="nav-links">
    <li><a href="#curriculum">Curriculum</a></li>
    <li><a href="#case-studies">Case Studies</a></li>
    <li><a href="#how-to-use">How to Use</a></li>
  </ul>
  <a href="#curriculum" class="nav-cta">Start Learning →</a>
</nav>

<!-- HERO -->
<section class="hero">
  <div class="free-pill">✦ 100% Free · No Account Needed · No Paywalls</div>
  <h1>Master System Design.<br><span class="accent">Build Anything at Scale.</span></h1>
  <p class="hero-sub">
    A complete, no-cost guide to system design interviews and distributed systems —
    written so every engineer on earth, regardless of income, can reach the top.
  </p>
  <div class="hero-actions">
    <a href="#curriculum" class="btn-primary">Explore the Curriculum</a>
    <a href="#why-free" class="btn-secondary">Why It's Free</a>
  </div>
  <div class="hero-stats">
    <div><div class="stat-val">83</div><div class="stat-lbl">Structured Lessons</div></div>
    <div><div class="stat-val">15+</div><div class="stat-lbl">Real-World Case Studies</div></div>
    <div><div class="stat-val">4</div><div class="stat-lbl">Core Modules</div></div>
    <div><div class="stat-val">₀</div><div class="stat-lbl">Cost to You, Forever</div></div>
  </div>
</section>

<!-- WHY FREE -->
<section id="why-free">
  <div class="center">
    <div class="section-label">The Mission</div>
    <h2 class="section-title">Knowledge is a right,<br>not a subscription.</h2>
    <p class="section-sub">
      Quality system design education has been locked behind paywalls for too long.
      Muhammad Qasim Academy exists to change that — permanently.
    </p>
  </div>
  <div class="why-grid">
    <div class="why-card">
      <div class="why-icon">🌍</div>
      <h3>Geography Shouldn't Limit You</h3>
      <p>Whether you're in Lahore, Lagos, or Lima — you deserve the same knowledge as engineers in Silicon Valley.</p>
    </div>
    <div class="why-card">
      <div class="why-icon">🔓</div>
      <h3>No Paywalls, Ever</h3>
      <p>No "free tier." No credit card. No upsell. Every lesson, every diagram, every concept — fully open.</p>
    </div>
    <div class="why-card">
      <div class="why-icon">📖</div>
      <h3>Real Depth, Not Summaries</h3>
      <p>Each topic is explained from first principles with diagrams, trade-offs, and interview-ready frameworks.</p>
    </div>
    <div class="why-card">
      <div class="why-icon">🚀</div>
      <h3>Interview-Ready Structure</h3>
      <p>Content is sequenced exactly how top companies interview — from fundamentals to FAANG-level design problems.</p>
    </div>
  </div>
</section>

<!-- CURRICULUM -->
<section id="curriculum" class="curriculum-bg">
  <div class="center" style="margin-bottom:3rem">
    <div class="section-label">Full Curriculum</div>
    <h2 class="section-title">Everything you need.<br>Structured, sequenced, free.</h2>
    <p class="section-sub">Four complete modules covering system design from first principles to FAANG-level problems.</p>
  </div>

  <div class="modules">

    <!-- MODULE 1 -->
    <div class="module open">
      <div class="module-header" onclick="this.parentElement.classList.toggle('open')">
        <span class="module-num">01</span>
        <span class="module-title">Introduction to System Design Interviews</span>
        <span class="module-meta">5 lessons</span>
        <span class="module-chevron">▼</span>
      </div>
      <div class="module-body">
        <ul class="lesson-list">
          <li><span class="lesson-dot"></span><span>What is a System Design Interview? — purpose, format, and what evaluators look for</span></li>
          <li><span class="lesson-dot"></span><span>Functional vs. Non-Functional Requirements — how to gather and frame them under time pressure</span></li>
          <li><span class="lesson-dot"></span><span>Back-of-the-Envelope Estimations — QPS, storage, bandwidth, and latency math</span></li>
          <li><span class="lesson-dot"></span><span>Common Mistakes to Avoid — skipping trade-offs, poor communication, tunnel vision</span></li>
          <li><span class="lesson-dot"></span><span>The Step-by-Step Interview Framework — a repeatable playbook for any open-ended question</span></li>
        </ul>
      </div>
    </div>

    <!-- MODULE 2 -->
    <div class="module">
      <div class="module-header" onclick="this.parentElement.classList.toggle('open')">
        <span class="module-num">02</span>
        <span class="module-title">Glossary of System Design Basics</span>
        <span class="module-meta">20 lessons</span>
        <span class="module-chevron">▼</span>
      </div>
      <div class="module-body">
        <ul class="lesson-list">
          <li><span class="lesson-dot"></span><span>System Design Building Blocks — the core components every large-scale system shares</span></li>
          <li><span class="lesson-dot"></span><span>Key Characteristics of Distributed Systems — scalability, reliability, availability, fault tolerance</span></li>
          <li><span class="lesson-dot"></span><span>Load Balancing — algorithms, health checks, and layer-4 vs layer-7 balancers</span></li>
          <li><span class="lesson-dot"></span><span>Load Balancing Algorithms — round robin, least connections, consistent hashing</span></li>
          <li><span class="lesson-dot"></span><span>Caching — strategies, eviction policies (LRU, LFU), cache invalidation</span></li>
          <li><span class="lesson-dot"></span><span>Data Partitioning — horizontal, vertical, range-based, hash-based sharding</span></li>
          <li><span class="lesson-dot"></span><span>Database Indexes — B-tree, composite, covering indexes and write trade-offs</span></li>
          <li><span class="lesson-dot"></span><span>Proxies — forward vs reverse proxy, use cases, and combined architectures</span></li>
          <li><span class="lesson-dot"></span><span>Redundancy & Replication — synchronous, asynchronous, and semi-synchronous</span></li>
          <li><span class="lesson-dot"></span><span>SQL vs. NoSQL — when to use each, consistency vs. flexibility</span></li>
          <li><span class="lesson-dot"></span><span>CAP Theorem — consistency, availability, partition tolerance trade-offs</span></li>
          <li><span class="lesson-dot"></span><span>PACELC Theorem — extending CAP with latency vs consistency trade-offs</span></li>
          <li><span class="lesson-dot"></span><span>Consistent Hashing — virtual nodes, ring architecture, dynamic scaling</span></li>
          <li><span class="lesson-dot"></span><span>Long-Polling vs WebSockets vs Server-Sent Events — choosing real-time protocols</span></li>
          <li><span class="lesson-dot"></span><span>Bloom Filters — probabilistic membership checks with minimal memory</span></li>
          <li><span class="lesson-dot"></span><span>Quorum — read/write quorum, distributed consensus, majority voting</span></li>
          <li><span class="lesson-dot"></span><span>Leader-Follower Architecture — replication, failover, and split-brain handling</span></li>
          <li><span class="lesson-dot"></span><span>Heartbeat — failure detection, keep-alive intervals, health monitoring</span></li>
          <li><span class="lesson-dot"></span><span>Checksums — CRC, MD5, SHA — data integrity in distributed transmission</span></li>
          <li><span class="lesson-dot"></span><span>Module Quiz — test your foundations before advancing</span></li>
        </ul>
      </div>
    </div>

    <!-- MODULE 3 -->
    <div class="module">
      <div class="module-header" onclick="this.parentElement.classList.toggle('open')">
        <span class="module-num">03</span>
        <span class="module-title">System Design Trade-offs</span>
        <span class="module-meta">23 lessons <span class="lesson-badge lb-new">New</span></span>
        <span class="module-chevron">▼</span>
      </div>
      <div class="module-body">
        <ul class="lesson-list">
          <li><span class="lesson-dot"></span><span>Why Trade-offs Define Senior Engineers — how to think and communicate like an architect</span></li>
          <li><span class="lesson-dot"></span><span>Strong vs. Eventual Consistency — latency, accuracy, and when each model is correct</span></li>
          <li><span class="lesson-dot"></span><span>Latency vs. Throughput — optimizing response time vs. data processing capacity</span></li>
          <li><span class="lesson-dot"></span><span>ACID vs. BASE Properties — transactional guarantees vs. availability and scale</span></li>
          <li><span class="lesson-dot"></span><span>Read-Through vs. Write-Through Cache — choosing the right caching strategy</span></li>
          <li><span class="lesson-dot"></span><span>Batch Processing vs. Stream Processing — scheduled jobs vs. real-time pipelines</span></li>
          <li><span class="lesson-dot"></span><span>Load Balancer vs. API Gateway — traffic distribution vs. request orchestration</span></li>
          <li><span class="lesson-dot"></span><span>API Gateway vs. Direct Service Exposure — centralized routing vs. low-latency direct access</span></li>
          <li><span class="lesson-dot"></span><span>Proxy vs. Reverse Proxy — client-side vs. server-side mediation</span></li>
          <li><span class="lesson-dot"></span><span>API Gateway vs. Reverse Proxy — routing logic, security, and when each applies</span></li>
          <li><span class="lesson-dot"></span><span>SQL vs. NoSQL (Deep Dive) — schema, ACID, CAP positioning, and access patterns</span></li>
          <li><span class="lesson-dot"></span><span>Primary-Replica vs. Peer-to-Peer Replication — consistency, failover, and write scaling</span></li>
          <li><span class="lesson-dot"></span><span>Data Compression vs. Deduplication — storage efficiency strategies compared</span></li>
          <li><span class="lesson-dot"></span><span>Server-Side vs. Client-Side Caching — control, stale data, and performance balance</span></li>
          <li><span class="lesson-dot"></span><span>REST vs. RPC — stateless resources vs. procedure calls, gRPC vs HTTP</span></li>
          <li><span class="lesson-dot"></span><span>Polling vs. Long-Polling vs. WebSockets vs. Webhooks — real-time delivery compared</span></li>
          <li><span class="lesson-dot"></span><span>CDN vs. Direct Server Serving — geographic distribution vs. origin control</span></li>
          <li><span class="lesson-dot"></span><span>Serverless vs. Traditional Server Architecture — auto-scaling vs. control</span></li>
          <li><span class="lesson-dot"></span><span>Stateful vs. Stateless Architecture — session handling, horizontal scaling, APIs</span></li>
          <li><span class="lesson-dot"></span><span>Hybrid Cloud vs. All-Cloud Storage — compliance, cost, and flexibility</span></li>
          <li><span class="lesson-dot"></span><span>Token Bucket vs. Leaky Bucket — rate limiting algorithms for traffic shaping</span></li>
          <li><span class="lesson-dot"></span><span>Read-Heavy vs. Write-Heavy Systems — design divergence and optimization patterns</span></li>
          <li><span class="lesson-dot"></span><span>Module Quiz — test your trade-off reasoning</span></li>
        </ul>
      </div>
    </div>

    <!-- MODULE 4 -->
    <div class="module">
      <div class="module-header" onclick="this.parentElement.classList.toggle('open')">
        <span class="module-num">04</span>
        <span class="module-title">System Design Problems — Full Walkthroughs</span>
        <span class="module-meta">35 lessons</span>
        <span class="module-chevron">▼</span>
      </div>
      <div class="module-body">
        <ul class="lesson-list">
          <li><span class="lesson-dot"></span><span>The Step-by-Step Interview Guide — requirements → estimation → design → deep dive</span></li>
          <li><span class="lesson-dot"></span><span>System Design Master Template — reusable framework for any problem</span></li>
          <li><span class="lesson-dot"></span><span>URL Shortening Service (like TinyURL) + Quiz</span></li>
          <li><span class="lesson-dot"></span><span>Pastebin Design + Quiz</span></li>
          <li><span class="lesson-dot"></span><span>Instagram Architecture + Quiz</span></li>
          <li><span class="lesson-dot"></span><span>Dropbox File Storage System + Quiz</span></li>
          <li><span class="lesson-dot"></span><span>Facebook Messenger / Chat System + Quiz</span></li>
          <li><span class="lesson-dot"></span><span>Twitter Feed Design + Quiz</span></li>
          <li><span class="lesson-dot"></span><span>YouTube / Netflix Video Platform + Quiz</span></li>
          <li><span class="lesson-dot"></span><span>Typeahead / Autocomplete Search + Quiz</span></li>
          <li><span class="lesson-dot"></span><span>API Rate Limiter Design + Quiz</span></li>
          <li><span class="lesson-dot"></span><span>Twitter Search Engine + Quiz</span></li>
          <li><span class="lesson-dot"></span><span>Web Crawler Architecture + Quiz</span></li>
          <li><span class="lesson-dot"></span><span>Facebook Newsfeed Ranking + Quiz</span></li>
          <li><span class="lesson-dot"></span><span>Yelp / Nearby Friends (Geo-Search) + Quiz</span></li>
          <li><span class="lesson-dot"></span><span>Uber Backend & Matching Engine + Quiz</span></li>
          <li><span class="lesson-dot"></span><span>Ticketmaster / Event Booking System + Quiz</span></li>
        </ul>
      </div>
    </div>

  </div>
</section>

<!-- TOPICS GRID -->
<section>
  <div class="center">
    <div class="section-label">Core Concepts</div>
    <h2 class="section-title">Every fundamental, covered in depth.</h2>
  </div>
  <div class="topics-grid">
    <div class="topic-chip"><span class="ti">⚖️</span> Load Balancing</div>
    <div class="topic-chip"><span class="ti">⚡</span> Caching Strategies</div>
    <div class="topic-chip"><span class="ti">🗄️</span> Database Sharding</div>
    <div class="topic-chip"><span class="ti">🔁</span> Replication</div>
    <div class="topic-chip"><span class="ti">📐</span> CAP Theorem</div>
    <div class="topic-chip"><span class="ti">🔗</span> Consistent Hashing</div>
    <div class="topic-chip"><span class="ti">🌐</span> CDN Architecture</div>
    <div class="topic-chip"><span class="ti">🔀</span> API Gateway</div>
    <div class="topic-chip"><span class="ti">📡</span> WebSockets & SSE</div>
    <div class="topic-chip"><span class="ti">🌸</span> Bloom Filters</div>
    <div class="topic-chip"><span class="ti">🏛️</span> Microservices</div>
    <div class="topic-chip"><span class="ti">🛡️</span> Rate Limiting</div>
    <div class="topic-chip"><span class="ti">🗃️</span> SQL vs NoSQL</div>
    <div class="topic-chip"><span class="ti">📊</span> Data Partitioning</div>
    <div class="topic-chip"><span class="ti">🔒</span> Quorum & Consensus</div>
    <div class="topic-chip"><span class="ti">🔄</span> Event-Driven Design</div>
    <div class="topic-chip"><span class="ti">📈</span> Scalability Patterns</div>
    <div class="topic-chip"><span class="ti">🧩</span> System Trade-offs</div>
  </div>
</section>

<!-- CASE STUDIES -->
<section id="case-studies" class="curriculum-bg">
  <div class="center">
    <div class="section-label">Real-World Case Studies</div>
    <h2 class="section-title">Design the systems you use every day.</h2>
    <p class="section-sub">Each case study is walked through end-to-end — requirements, estimation, architecture, and bottlenecks.</p>
  </div>
  <div class="cases-grid">
    <div class="case-card"><div class="case-icon">🔗</div><div><h4>TinyURL</h4><p>URL shortening, base-62 encoding, redirect at scale</p></div></div>
    <div class="case-card"><div class="case-icon">📸</div><div><h4>Instagram</h4><p>Photo upload, CDN, feed generation, social graph</p></div></div>
    <div class="case-card"><div class="case-icon">📦</div><div><h4>Dropbox</h4><p>File chunking, sync, deduplication, conflict resolution</p></div></div>
    <div class="case-card"><div class="case-icon">💬</div><div><h4>Facebook Messenger</h4><p>Real-time messaging, presence, offline delivery</p></div></div>
    <div class="case-card"><div class="case-icon">🐦</div><div><h4>Twitter</h4><p>Tweet fanout, timelines, trending, search indexing</p></div></div>
    <div class="case-card"><div class="case-icon">▶️</div><div><h4>YouTube / Netflix</h4><p>Video encoding, adaptive bitrate, CDN, recommendations</p></div></div>
    <div class="case-card"><div class="case-icon">🔍</div><div><h4>Typeahead Search</h4><p>Trie vs inverted index, latency, prefix caching</p></div></div>
    <div class="case-card"><div class="case-icon">🚗</div><div><h4>Uber Backend</h4><p>Matching engine, geospatial indexing, surge pricing</p></div></div>
    <div class="case-card"><div class="case-icon">🕷️</div><div><h4>Web Crawler</h4><p>BFS/DFS crawling, politeness, deduplication, storage</p></div></div>
    <div class="case-card"><div class="case-icon">📰</div><div><h4>Facebook Newsfeed</h4><p>Ranking, fanout strategies, edge cases at 1B users</p></div></div>
    <div class="case-card"><div class="case-icon">📍</div><div><h4>Yelp / Nearby Friends</h4><p>Geohashing, Quadtree, proximity search at scale</p></div></div>
    <div class="case-card"><div class="case-icon">🎟️</div><div><h4>Ticketmaster</h4><p>Seat locking, high-concurrency booking, fairness</p></div></div>
  </div>
</section>

<!-- HOW TO USE -->
<section id="how-to-use">
  <div class="center">
    <div class="section-label">Get Started</div>
    <h2 class="section-title">Ready in three steps. No setup needed.</h2>
  </div>
  <div class="steps">
    <div class="step">
      <div class="step-circle">1</div>
      <h3>Open the Repository</h3>
      <p>Visit the Muhammad Qasim Academy GitHub repo — no account, no sign-up required to read.</p>
    </div>
    <div class="step">
      <div class="step-circle">2</div>
      <h3>Pick Your Module</h3>
      <p>Start at Module 1 if you're new. Jump to trade-offs or case studies if you have a specific interview soon.</p>
    </div>
    <div class="step">
      <div class="step-circle">3</div>
      <h3>Build & Practice</h3>
      <p>Work through each design problem, attempt the quiz, then re-read the walkthrough to close your gaps.</p>
    </div>
    <div class="step">
      <div class="step-circle">⭐</div>
      <h3>Star & Share</h3>
      <p>If this helped you, star the repo and share it. Every share puts free education in front of one more engineer.</p>
    </div>
  </div>
</section>

<!-- CTA -->
<div class="cta-banner">
  <h2>Start learning right now —<br>it costs nothing.</h2>
  <p>No paywalls. No emails. No limits. Just knowledge, for every engineer on the planet.</p>
  <a href="#curriculum" class="btn-primary">Begin with Module 1 →</a>
</div>

<!-- FOOTER -->
<footer>
  <div class="logo">Muhammad Qasim <span>Academy</span></div>
  <div class="footer-links">
    <a href="#curriculum">Curriculum</a>
    <a href="#case-studies">Case Studies</a>
    <a href="#why-free">Why Free</a>
    <a href="#how-to-use">How to Use</a>
  </div>
  <p class="copy">Built with ❤️ by Muhammad Qasim — Free forever, for every engineer on earth.</p>
</footer>

<script>
  // Smooth accordion — close others when one opens
  document.querySelectorAll('.module-header').forEach(header => {
    header.addEventListener('click', () => {
      const mod = header.parentElement;
      const isOpen = mod.classList.contains('open');
      // allow multiple open — toggle only this
      mod.classList.toggle('open', !isOpen);
    });
  });
</script>
</body>
</html>
