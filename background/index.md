---
layout: page
title: Background
category: Background
body_class: background-page
subtitle: Chemical engineering as the science of delivery.
---

<style>
/* Background page — scoped to .bp and aligned to the main portfolio CSS token system */
.bp{
  width:min(980px, calc(100% - 40px));
  margin:0 auto;
  padding:clamp(88px, 8vw, 118px) 0 88px;
  color:var(--ink, #111827);
  font-family:Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
}
.bp *{box-sizing:border-box}
.bp .sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);white-space:nowrap;border:0}
.bp p,.bp h1,.bp h2,.bp h3{margin:0}
.bp p{color:var(--body, #334155);font-size:1.01rem;line-height:1.76;letter-spacing:-.01em}
.bp .section{margin-top:clamp(56px, 7vw, 84px)}
.bp .eyebrow{
  display:inline-flex;
  align-items:center;
  gap:8px;
  margin:0 0 14px;
  color:var(--green, #3e9a75);
  font-family:var(--mono, "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace);
  font-size:.68rem;
  font-weight:780;
  letter-spacing:.145em;
  text-transform:uppercase;
}
.bp .eyebrow::before{
  content:"";
  width:7px;
  height:7px;
  border-radius:999px;
  background:var(--green, #3e9a75);
  box-shadow:0 0 0 4px rgba(62,154,117,.10);
}
.bp h1{
  max-width:840px;
  color:var(--ink, #111827);
  font-size:clamp(3.05rem, 7.3vw, 6.35rem);
  line-height:.94;
  letter-spacing:-.082em;
  text-wrap:balance;
}
.bp h2{
  max-width:780px;
  color:var(--ink, #111827);
  font-size:clamp(2rem, 4.4vw, 3.75rem);
  line-height:1;
  letter-spacing:-.068em;
  text-wrap:balance;
}
.bp .subline{
  max-width:690px;
  margin-top:22px;
  color:#254048;
  font-size:clamp(1.08rem, 1.55vw, 1.26rem);
  line-height:1.68;
  letter-spacing:-.025em;
}
.bp .hero-shell{
  position:relative;
  display:grid;
  grid-template-columns:minmax(0,1.12fr) minmax(270px,.62fr);
  gap:clamp(28px, 5vw, 58px);
  align-items:end;
}
.bp .hero-shell::before{
  content:"";
  position:absolute;
  inset:-28px -24px auto auto;
  width:280px;
  height:280px;
  border-radius:999px;
  background:radial-gradient(circle, rgba(59,150,215,.10), transparent 68%);
  pointer-events:none;
  z-index:-1;
}
.bp .intro-copy{
  display:grid;
  gap:1.06rem;
  margin-top:30px;
  max-width:735px;
}

/* ── Identity card ─────────────────────────────────────────────────────── */
.bp .identity-card{
  position:relative;
  overflow:hidden;
  border:1px solid var(--line, rgba(15,23,42,.095));
  border-radius:34px;
  background:linear-gradient(135deg, rgba(255,255,255,.94), rgba(239,248,247,.78));
  box-shadow:var(--shadow-soft, 0 10px 30px rgba(15,35,55,.055));
}
.bp .identity-card::before{
  content:"";
  position:absolute;
  inset:0;
  background:
    linear-gradient(rgba(9,51,56,.045) 1px, transparent 1px),
    linear-gradient(90deg, rgba(9,51,56,.035) 1px, transparent 1px);
  background-size:36px 36px;
  opacity:.45;
  pointer-events:none;
}
.bp .identity-visual{
  position:relative;
  min-height:200px;
  display:grid;
  place-items:center;
  border-bottom:1px solid var(--line, rgba(15,23,42,.095));
}
.bp .identity-visual.identity-photo-wrap{
  min-height:0;
  display:block;
  border-bottom:1px solid var(--line, rgba(15,23,42,.095));
}
.bp .identity-photo{
  position:relative;
  z-index:1;
  display:block;
  width:100%;
  aspect-ratio:4 / 5;
  object-fit:cover;
  object-position:center;
}
.bp .identity-meta{
  position:relative;
  padding:21px 22px 23px;
}
.bp .identity-name{
  margin:0 0 6px;
  color:var(--ink, #111827);
  font-size:1.18rem;
  line-height:1.05;
  font-weight:820;
  letter-spacing:-.055em;
}
.bp .identity-line{
  margin:0;
  color:var(--muted, #64748b);
  font-size:.9rem;
  line-height:1.48;
}
.bp .identity-proof{
  display:flex;
  flex-wrap:wrap;
  gap:7px;
  margin-top:16px;
}
.bp .mini-chip,.bp .proof-pill,.bp .tag{
  display:inline-flex;
  align-items:center;
  border:1px solid var(--line, rgba(15,23,42,.095));
  border-radius:999px;
  background:rgba(255,255,255,.74);
  color:var(--graphite, #20383c);
  font-family:var(--mono, "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace);
  font-size:.61rem;
  font-weight:760;
  letter-spacing:.07em;
  line-height:1.2;
  text-transform:uppercase;
}
.bp .mini-chip{padding:7px 9px}

/* ── Pull quote ─────────────────────────────────────────────────────────── */
.bp .pull-quote{
  margin:34px 0 0;
  padding:24px 26px;
  border:1px solid rgba(23,109,155,.13);
  border-radius:28px;
  background:linear-gradient(135deg, rgba(255,255,255,.92), rgba(234,246,255,.58));
  box-shadow:var(--shadow-soft, 0 10px 30px rgba(15,35,55,.055));
}
.bp .pull-quote p{
  max-width:840px;
  color:var(--ink, #111827);
  font-size:clamp(1.32rem, 2.4vw, 2.05rem);
  line-height:1.23;
  letter-spacing:-.055em;
  font-weight:780;
}

/* ── Focus card ─────────────────────────────────────────────────────────── */
.bp .focus-card{
  margin-top:28px;
  padding:24px;
  border:1px solid var(--line, rgba(15,23,42,.095));
  border-radius:30px;
  background:rgba(255,255,255,.88);
  box-shadow:var(--shadow-soft, 0 10px 30px rgba(15,35,55,.055));
}
.bp .focus-grid{
  display:grid;
  grid-template-columns:minmax(0,.95fr) minmax(0,1.05fr);
  gap:24px;
  align-items:start;
}
.bp .focus-kicker{
  margin:0 0 8px;
  color:var(--green, #3e9a75);
  font-family:var(--mono, "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace);
  font-size:.66rem;
  font-weight:780;
  letter-spacing:.13em;
  text-transform:uppercase;
}
.bp .focus-title{
  margin:0 0 10px;
  color:var(--ink, #111827);
  font-size:1.23rem;
  line-height:1.18;
  letter-spacing:-.04em;
  font-weight:820;
}
.bp .focus-card p{font-size:.96rem;color:var(--muted, #64748b)}
.bp .proof-list{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:9px;
}
.bp .proof-pill{
  min-height:34px;
  padding:8px 10px;
  background:#fff;
  border-color:rgba(23,109,155,.13);
}
.bp .proof-pill::before{
  content:"";
  width:6px;
  height:6px;
  margin-right:7px;
  border-radius:999px;
  background:var(--blue-deep, #176d9b);
  box-shadow:0 0 0 3px rgba(23,109,155,.09);
  flex-shrink:0;
}

/* ── Bridge strip ───────────────────────────────────────────────────────── */
/* overflow removed — transparent children don't break border-radius;
   ::after arrows are now visible                                          */
.bp .bridge-strip{
  display:grid;
  grid-template-columns:repeat(4,minmax(0,1fr));
  gap:0;
  margin-top:24px;
  border:1px solid var(--line, rgba(15,23,42,.095));
  border-radius:26px;
  background:linear-gradient(135deg, rgba(255,255,255,.94), rgba(239,248,247,.70));
}
.bp .bridge-step{
  position:relative;
  min-height:128px;
  padding:20px 18px;
  border-right:1px solid var(--line, rgba(15,23,42,.095));
}
.bp .bridge-step:first-child{border-radius:26px 0 0 26px}
.bp .bridge-step:last-child{border-right:0;border-radius:0 26px 26px 0}
.bp .bridge-step:not(:last-child)::after{
  content:"→";
  position:absolute;
  right:-9px;
  top:24px;
  z-index:2;
  display:grid;
  place-items:center;
  width:18px;
  height:18px;
  border:1px solid var(--line, rgba(15,23,42,.095));
  border-radius:999px;
  background:#fff;
  color:var(--muted, #64748b);
  font-family:var(--mono, "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace);
  font-size:.62rem;
}
.bp .bridge-step strong{
  display:block;
  margin-bottom:8px;
  color:var(--ink, #111827);
  font-family:var(--mono, "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace);
  font-size:.7rem;
  letter-spacing:.09em;
  text-transform:uppercase;
}
.bp .bridge-step span{
  display:block;
  color:var(--muted, #64748b);
  font-size:.91rem;
  line-height:1.48;
}

/* ── Media cards (sci-fi shelf) ─────────────────────────────────────────── */
.bp .media-grid{
  display:grid;
  grid-template-columns:repeat(3,minmax(0,1fr));
  gap:14px;
  margin-top:24px;
}
.bp .media-card{
  position:relative;
  overflow:hidden;
  min-height:236px;
  padding:19px;
  border:1px solid var(--line, rgba(15,23,42,.095));
  border-radius:26px;
  background:rgba(255,255,255,.88);
  box-shadow:var(--shadow-soft, 0 10px 30px rgba(15,35,55,.055));
}
/* Distinct solid color per card */
.bp .media-card::before{
  content:"";
  position:absolute;
  left:0;
  right:0;
  top:0;
  height:5px;
}
.bp .media-card:nth-child(1)::before{background:var(--blue-deep, #176d9b);opacity:.70}
.bp .media-card:nth-child(2)::before{background:var(--green, #3e9a75);opacity:.70}
.bp .media-card:nth-child(3)::before{background:var(--solar, #d4a72c);opacity:.76}
.bp .tag{
  padding:6px 8px;
  color:var(--blue-deep, #176d9b);
  background:rgba(234,246,255,.72);
}
.bp .media-card h3{
  margin:18px 0 6px;
  color:var(--ink, #111827);
  font-size:1.3rem;
  line-height:1.03;
  letter-spacing:-.052em;
}
.bp .media-year{
  display:block;
  margin-bottom:14px;
  color:var(--faint, #94a3b8);
  font-family:var(--mono, "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace);
  font-size:.68rem;
  letter-spacing:.08em;
}
.bp .media-card p{font-size:.92rem;line-height:1.58;color:var(--muted, #64748b)}
.bp .infra-note{
  margin-top:16px;
  padding:18px 20px;
  border-top:1px solid var(--line, rgba(15,23,42,.095));
  border-bottom:1px solid var(--line, rgba(15,23,42,.095));
  background:linear-gradient(90deg, rgba(255,255,255,.60), rgba(239,248,247,.62), rgba(255,255,255,.60));
}
.bp .infra-note p{max-width:830px;color:var(--body, #334155)}

/* ── Compare table ──────────────────────────────────────────────────────── */
.bp .compare-table{
  margin-top:24px;
  border:1px solid var(--line, rgba(15,23,42,.095));
  border-radius:28px;
  overflow:hidden;
  background:#fff;
  box-shadow:var(--shadow-soft, 0 10px 30px rgba(15,35,55,.055));
}
.bp .compare-head,.bp .compare-row{
  display:grid;
  grid-template-columns:.8fr .9fr 1.3fr;
}
.bp .compare-head div{
  padding:14px 16px;
  border-right:1px solid var(--line, rgba(15,23,42,.095));
  background:#f0faf9;
  color:var(--graphite, #20383c);
  font-family:var(--mono, "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace);
  font-size:.66rem;
  font-weight:780;
  letter-spacing:.09em;
  text-transform:uppercase;
}
.bp .compare-head div:last-child{border-right:0}
.bp .compare-row{border-top:1px solid var(--line, rgba(15,23,42,.095))}
.bp .compare-row div{
  padding:15px 16px;
  border-right:1px solid var(--line, rgba(15,23,42,.095));
  color:var(--body, #334155);
  font-size:.95rem;
  line-height:1.5;
}
.bp .compare-row div:last-child{border-right:0}
.bp .compare-row div strong{
  color:var(--ink, #111827);
  font-family:var(--mono, "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace);
  font-size:.66rem;
  letter-spacing:.075em;
  text-transform:uppercase;
}
.bp .compare-row div:nth-child(1){
  color:var(--muted, #64748b);
  background:rgba(248,251,251,.65);
}
.bp .compare-row div:nth-child(2){
  color:var(--ink, #111827);
  font-weight:720;
}

/* ── System diagram ─────────────────────────────────────────────────────── */
.bp .system-diagram{
  display:grid;
  grid-template-columns:minmax(0,.82fr) minmax(0,1.18fr);
  gap:26px;
  align-items:center;
  margin-top:24px;
  padding:26px;
  border:1px solid var(--line, rgba(15,23,42,.095));
  border-radius:32px;
  background:linear-gradient(135deg, rgba(255,255,255,.94), rgba(239,248,247,.74));
  box-shadow:var(--shadow-soft, 0 10px 30px rgba(15,35,55,.055));
}
.bp .process-map{
  position:relative;
  min-height:318px;
  display:grid;
  grid-template-columns:1fr;
  gap:10px;
  padding:18px;
  border:1px solid var(--line, rgba(15,23,42,.095));
  border-radius:26px;
  background:
    linear-gradient(rgba(9,51,56,.04) 1px, transparent 1px),
    linear-gradient(90deg, rgba(9,51,56,.03) 1px, transparent 1px),
    linear-gradient(135deg, #fff, #f3fbfb);
  background-size:28px 28px, 28px 28px, auto;
  overflow:hidden;
}
.bp .process-map::before{
  content:"";
  position:absolute;
  inset:18px auto 18px 30px;
  width:1px;
  background:linear-gradient(180deg, rgba(23,109,155,.18), rgba(23,109,155,.42), rgba(62,154,117,.38));
  pointer-events:none;
}
.bp .process-node{
  position:relative;
  z-index:1;
  display:grid;
  gap:5px;
  padding:13px 14px 13px 22px;
  border:1px solid rgba(15,23,42,.09);
  border-radius:20px;
  background:rgba(255,255,255,.88);
  box-shadow:0 8px 20px rgba(15,35,55,.045);
}
.bp .process-node::before{
  content:"";
  position:absolute;
  left:9px;
  top:18px;
  width:8px;
  height:8px;
  border-radius:999px;
  background:var(--blue-deep, #176d9b);
  box-shadow:0 0 0 5px rgba(23,109,155,.08);
}
.bp .process-node.transport::before,.bp .process-node.rule::before{
  background:var(--green, #3e9a75);
  box-shadow:0 0 0 5px rgba(62,154,117,.08);
}
.bp .process-node span{
  color:var(--blue-deep, #176d9b);
  font-family:var(--mono, "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace);
  font-size:.58rem;
  font-weight:780;
  letter-spacing:.09em;
  text-transform:uppercase;
}
.bp .process-node.rule span,.bp .process-node.transport span{color:var(--green, #3e9a75)}
.bp .process-node strong{
  color:var(--ink, #111827);
  font-size:.94rem;
  line-height:1.16;
  letter-spacing:-.025em;
}
.bp .process-node small{
  color:var(--muted, #64748b);
  font-size:.78rem;
  line-height:1.38;
}
/* Arrow spans inside process-map */
.bp .process-map .pm-arr{
  position:relative;
  z-index:2;
  display:block;
  width:18px;
  height:18px;
  margin:-2px 0 -2px 3px;
  border:1px solid rgba(23,109,155,.14);
  border-radius:999px;
  background:#fff;
}
.bp .process-map .pm-arr::before{
  content:"↓";
  position:absolute;
  inset:0;
  display:grid;
  place-items:center;
  color:var(--blue-deep, #176d9b);
  font-family:var(--mono, "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace);
  font-size:.58rem;
  font-weight:780;
}
.bp .diagram-copy h3{
  margin:0 0 10px;
  color:var(--ink, #111827);
  font-size:clamp(1.45rem, 2.8vw, 2.35rem);
  line-height:1.05;
  letter-spacing:-.058em;
}
.bp .diagram-copy p{color:var(--muted, #64748b)}

/* ── Process loop grid ──────────────────────────────────────────────────── */
/* overflow removed — transparent children don't break border-radius;
   ::after arrows are now visible                                          */
.bp .loop-grid{
  display:grid;
  grid-template-columns:repeat(4,minmax(0,1fr));
  gap:0;
  margin-top:24px;
  border:1px solid var(--line, rgba(15,23,42,.095));
  border-radius:28px;
  background:#fff;
  box-shadow:var(--shadow-soft, 0 10px 30px rgba(15,35,55,.055));
}
.bp .loop-step{
  position:relative;
  min-height:220px;
  padding:22px 18px;
  border-right:1px solid var(--line, rgba(15,23,42,.095));
}
.bp .loop-step:first-child{border-radius:28px 0 0 28px}
.bp .loop-step:last-child{border-right:0;border-radius:0 28px 28px 0}
.bp .loop-step:not(:last-child)::after{
  content:"→";
  position:absolute;
  right:-9px;
  top:28px;
  z-index:2;
  display:grid;
  place-items:center;
  width:18px;
  height:18px;
  border:1px solid var(--line, rgba(15,23,42,.095));
  border-radius:999px;
  background:#fff;
  color:var(--muted, #64748b);
  font-family:var(--mono, "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace);
  font-size:.62rem;
}
.bp .loop-n{
  display:block;
  margin-bottom:12px;
  color:var(--faint, #94a3b8);
  font-family:var(--mono, "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace);
  font-size:.66rem;
  font-weight:780;
  letter-spacing:.1em;
}
.bp .loop-step h3{
  margin:0 0 8px;
  color:var(--ink, #111827);
  font-size:1.15rem;
  line-height:1.06;
  letter-spacing:-.04em;
}
.bp .loop-step p{
  color:var(--muted, #64748b);
  font-size:.91rem;
  line-height:1.52;
}
.bp .loop-example{
  display:block;
  margin-top:15px;
  padding-top:13px;
  border-top:1px solid var(--line, rgba(15,23,42,.095));
  color:var(--body, #334155);
  font-family:var(--mono, "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace);
  font-size:.62rem;
  font-weight:720;
  letter-spacing:.045em;
  line-height:1.55;
  text-transform:uppercase;
}

/* ── Open question ──────────────────────────────────────────────────────── */
.bp .open-question{
  margin-top:24px;
  padding:26px;
  border:1px solid rgba(23,109,155,.15);
  border-radius:30px;
  background:linear-gradient(135deg, rgba(255,255,255,.94), rgba(234,246,255,.60));
  box-shadow:var(--shadow-soft, 0 10px 30px rgba(15,35,55,.055));
}
.bp .q-label{
  margin:0 0 10px;
  color:var(--blue-deep, #176d9b);
  font-family:var(--mono, "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace);
  font-size:.68rem;
  font-weight:780;
  letter-spacing:.13em;
  text-transform:uppercase;
}
.bp .q-main{
  max-width:840px;
  margin:0 0 14px;
  color:var(--ink, #111827);
  font-size:clamp(1.55rem, 3vw, 2.45rem);
  line-height:1.12;
  letter-spacing:-.06em;
  font-weight:820;
}
.bp .q-body{max-width:780px;color:var(--muted, #64748b);margin-bottom:16px}
.bp .q-link{
  display:inline-flex;
  align-items:center;
  color:var(--blue-deep, #176d9b);
  font-family:var(--mono, "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace);
  font-size:.72rem;
  font-weight:720;
  letter-spacing:.05em;
  text-decoration:none;
  border-bottom:1px solid rgba(23,109,155,.28);
  padding-bottom:1px;
  transition:border-color 150ms ease, opacity 150ms ease;
}
.bp .q-link:hover{opacity:.72;border-color:rgba(23,109,155,.55)}

/* ── Timeline ───────────────────────────────────────────────────────────── */
.bp .timeline{
  display:grid;
  grid-template-columns:repeat(4,minmax(0,1fr));
  gap:0;
  margin-top:34px;
  padding:22px 0 4px;
  border-top:1px solid var(--line, rgba(15,23,42,.095));
}
.bp .time-step{
  position:relative;
  padding:0 18px;
  text-align:center;
}
.bp .time-step:not(:last-child)::after{
  content:"";
  position:absolute;
  top:8px;
  left:50%;
  width:100%;
  height:1px;
  background:linear-gradient(90deg, rgba(23,109,155,.22), rgba(62,154,117,.20));
}
.bp .time-dot{
  position:relative;
  z-index:2;
  display:block;
  width:16px;
  height:16px;
  margin:0 auto 12px;
  border:4px solid var(--blue-deep, #176d9b);
  border-radius:999px;
  background:#fff;
  box-shadow:0 0 0 7px rgba(23,109,155,.07);
}
.bp .time-step.now .time-dot{border-color:var(--green, #3e9a75);box-shadow:0 0 0 7px rgba(62,154,117,.08)}
.bp .time-place{
  display:block;
  color:var(--ink, #111827);
  font-weight:820;
  letter-spacing:-.035em;
  line-height:1.1;
}
.bp .time-note{
  display:block;
  margin-top:5px;
  color:var(--muted, #64748b);
  font-size:.86rem;
  line-height:1.35;
}

/* ── CTAs ────────────────────────────────────────────────────────────────── */
.bp .cta-row{
  display:flex;
  flex-wrap:wrap;
  gap:12px;
  margin-top:34px;
}
.bp .cta{
  display:inline-flex;
  align-items:center;
  min-height:46px;
  padding:12px 17px;
  border:1px solid var(--line-strong, rgba(15,23,42,.16));
  border-radius:999px;
  background:rgba(255,255,255,.84);
  color:#15373b;
  font-size:.94rem;
  font-weight:790;
  text-decoration:none;
  transition:transform 150ms ease, box-shadow 150ms ease, border-color 150ms ease;
}
.bp .cta:hover{
  transform:translateY(-2px);
  border-color:rgba(23,109,155,.28);
  box-shadow:var(--shadow-soft, 0 10px 30px rgba(15,35,55,.055));
}
.bp .cta.primary{
  border-color:transparent;
  color:#fff;
  background:linear-gradient(135deg, #176d9b, #2fb6ce);
  box-shadow:0 14px 28px rgba(13,142,177,.18);
}
.bp .cta.primary:hover{color:#fff;box-shadow:0 18px 34px rgba(13,142,177,.22)}

/* ── Hover transitions ──────────────────────────────────────────────────── */
@media (prefers-reduced-motion:no-preference){
  .bp .identity-card,.bp .focus-card,.bp .media-card,.bp .system-diagram,.bp .open-question,.bp .cta{
    transition:transform 160ms ease, border-color 160ms ease, box-shadow 160ms ease;
  }
  .bp .identity-card:hover,.bp .focus-card:hover,.bp .media-card:hover,.bp .system-diagram:hover,.bp .open-question:hover{
    transform:translateY(-3px);
    border-color:rgba(23,109,155,.18);
    box-shadow:var(--shadow-card, 0 18px 44px rgba(15,35,55,.09));
  }
}

/* ── Responsive ─────────────────────────────────────────────────────────── */
@media (max-width:900px){
  .bp{width:min(100% - 32px, 980px);padding-top:96px}
  .bp .hero-shell,.bp .focus-grid,.bp .system-diagram{grid-template-columns:1fr}
  .bp .process-map{min-height:0}
  .bp .identity-card{max-width:520px}
  .bp .media-grid,.bp .loop-grid,.bp .bridge-strip{grid-template-columns:1fr}
  .bp .bridge-step,.bp .loop-step{min-height:0;border-right:0;border-bottom:1px solid var(--line, rgba(15,23,42,.095))}
  .bp .bridge-step:first-child,.bp .loop-step:first-child{border-radius:26px 26px 0 0}
  .bp .bridge-step:last-child,.bp .loop-step:last-child{border-radius:0 0 26px 26px;border-bottom:0}
  .bp .bridge-step:not(:last-child)::after{content:"↓";right:auto;left:22px;top:auto;bottom:-10px}
  .bp .loop-step:not(:last-child)::after{content:"↓";right:auto;left:18px;top:auto;bottom:-10px}
  .bp .compare-head,.bp .compare-row{grid-template-columns:1fr}
  .bp .compare-head div,.bp .compare-row div{border-right:0;border-bottom:1px solid var(--line, rgba(15,23,42,.095))}
  .bp .compare-head div:last-child,.bp .compare-row div:last-child{border-bottom:0}
  .bp .proof-list{grid-template-columns:1fr}
}
@media (max-width:660px){
  .bp{width:min(100% - 28px, 980px);padding-top:86px}
  .bp h1{font-size:clamp(2.7rem, 12vw, 4.35rem);line-height:.97;letter-spacing:-.074em}
  .bp h2{font-size:clamp(1.9rem, 9vw, 3rem)}
  .bp .pull-quote,.bp .focus-card,.bp .open-question,.bp .system-diagram{padding:20px}
  .bp .timeline{grid-template-columns:1fr;gap:18px}
  .bp .time-step{text-align:left;display:grid;grid-template-columns:26px 1fr;column-gap:10px}
  .bp .time-step:not(:last-child)::after{display:none}
  .bp .time-dot{margin:2px 0 0}
  .bp .time-note{grid-column:2}
}
</style>

<main class="bp motion-enabled">
  <span class="sr-only">Nathan Anderson's background and philosophy as a process engineer</span>

  <section class="hero-shell" aria-label="Background introduction">
    <div>
      <div class="eyebrow">Background</div>
      <h1>Chemical engineering as the science of delivery.</h1>
      <p class="subline">Discovery shows what is possible. Delivery proves what can be repeated.</p>

      <div class="intro-copy">
        <p>I was adopted from Incheon at seven months old and grew up in small-town Minnesota — too Korean for some rooms, not Korean enough for others. That in-between feeling made me notice systems early: who they were built for, who had to adapt to them, and whose futures they made possible.</p>
        <p>That is why I was pulled toward worlds like <em>Ghost in the Shell</em>, <em>The Matrix</em>, and <em>Final Fantasy VII</em>. They did not make me want gadgets. They made me interested in infrastructure: the materials, interfaces, energy systems, and control layers that determine whether technology becomes part of ordinary life.</p>
        <p>The future often appears first as a fragile lab result. The harder question is what it takes to make that result reliable enough to leave the lab.</p>
      </div>
    </div>

    <div class="identity-card" aria-label="Nathan Anderson technical identity card">
      <div class="identity-visual identity-photo-wrap">
        <img class="identity-photo" src="{{ '/assets/images/nathan-anderson-headshot.jpg' | relative_url }}" alt="Portrait of Nathan Anderson">
      </div>
      <div class="identity-meta">
        <p class="identity-name">Nathan Anderson</p>
        <p class="identity-line">Chemical &amp; Biomolecular Engineering · Georgia Tech</p>
        <div class="identity-proof" aria-label="Portfolio focus areas">
          <span class="mini-chip">Process development</span>
          <span class="mini-chip">Printed electronics</span>
          <span class="mini-chip">Manufacturable design rules</span>
        </div>
      </div>
    </div>
  </section>

  <a class="scroll-cue featured-case-cue background-scroll-cue" href="#current-focus" aria-label="Scroll to current technical focus">
    <span>Current technical focus</span>
    <strong aria-hidden="true">↓</strong>
  </a>

  <div class="pull-quote reveal" style="--reveal-delay: 40ms">
    <p>Chemical engineering is my answer: the discipline that turns physical phenomena into processes that can be measured, repeated, scaled, and transferred — for people who were not in the room where the breakthrough happened.</p>
  </div>

  <section id="current-focus" class="focus-card reveal" aria-label="Current technical focus" style="--reveal-delay: 80ms">
    <div class="focus-grid">
      <div>
        <p class="focus-kicker">Current technical focus</p>
        <h2 class="focus-title">Micromodular printed electronics process development</h2>
        <p>In the Filler Lab at Georgia Tech, I study how droplet transport, substrate boundary conditions, and measurement workflows control where suspended microdevices land — then turn that behavior into placement metrics and substrate design rules.</p>
      </div>
      <div class="proof-list" aria-label="Current proof points">
        <span class="proof-pill">Image-analysis workflows</span>
        <span class="proof-pill">Substrate/backing comparisons</span>
        <span class="proof-pill">Edge/center accumulation metrics</span>
        <span class="proof-pill">Wetting + imbibition dynamics</span>
        <span class="proof-pill">Python/JMP metric extraction</span>
        <span class="proof-pill">Optical microscopy</span>
      </div>
    </div>
  </section>

  <section class="section reveal" aria-label="Infrastructure origins" style="--reveal-delay: 120ms">
    <div class="eyebrow">Where the infrastructure question started</div>
    <h2>Fiction made the stakes of infrastructure feel personal.</h2>
    <p class="subline">The stories that shaped me were not just about advanced technology. They made me look for the systems beneath the surface: materials, energy, interfaces, and control layers.</p>

    <div class="media-grid reveal" style="--reveal-delay: 180ms">
      <article class="media-card">
        <span class="tag">Human-machine infrastructure</span>
        <h3>Ghost in the Shell</h3>
        <span class="media-year">Shirow · 1989</span>
        <p>Technology as infrastructure close enough to reshape identity, labor, and the body.</p>
      </article>
      <article class="media-card">
        <span class="tag">Control systems + interfaces</span>
        <h3>The Matrix</h3>
        <span class="media-year">Wachowskis · 1999</span>
        <p>A world defined by invisible architecture: interfaces, networks, feedback loops, and failure modes.</p>
      </article>
      <article class="media-card">
        <span class="tag">Energy systems + social cost</span>
        <h3>Final Fantasy VII</h3>
        <span class="media-year">Sakaguchi · 1997</span>
        <p>A city powered by the planet's lifeblood. Energy systems as moral infrastructure with cultural cost.</p>
      </article>
    </div>

    <div class="infra-note">
      <p>Those worlds made technology feel less like invention and more like infrastructure: something designed, scaled, maintained, and eventually lived inside.</p>
    </div>
  </section>

  <section class="section reveal" aria-label="Why process development" style="--reveal-delay: 160ms">
    <div class="eyebrow">Why process development</div>
    <h2>A breakthrough is not finished when it works once.</h2>
    <p class="subline">I want to work where the hard part is not proving that something can happen, but defining the conditions under which it can happen again.</p>

    <div class="compare-table reveal" aria-label="Discovery to delivery comparison table" style="--reveal-delay: 200ms">
      <div class="compare-head">
        <div>Discovery</div>
        <div>Delivery</div>
        <div>What this looks like in my work</div>
      </div>
      <div class="compare-row">
        <div>First demonstration in a lab</div>
        <div>Repeatable process window</div>
        <div><strong>Metric:</strong> droplet behavior → deposition outcome</div>
      </div>
      <div class="compare-row">
        <div>Interesting result</div>
        <div>Usable manufacturing criteria</div>
        <div><strong>Metric:</strong> edge/center accumulation + repeatability</div>
      </div>
      <div class="compare-row">
        <div>Lab-specific conditions</div>
        <div>Substrate-agnostic design rules</div>
        <div><strong>Input space:</strong> AAO, glass, backing layers, and surface boundary conditions</div>
      </div>
      <div class="compare-row">
        <div>Proof of concept</div>
        <div>Assembly with measurable placement fidelity</div>
        <div><strong>Criterion:</strong> physical transport → placement fidelity</div>
      </div>
      <div class="compare-row">
        <div>Reported result</div>
        <div>Reproducible method</div>
        <div><strong>Output:</strong> reproducible measurement framework</div>
      </div>
    </div>
  </section>

  <section class="section reveal" aria-label="Georgia Tech and lab work" style="--reveal-delay: 200ms">
    <div class="eyebrow">Georgia Tech → the lab</div>
    <h2>I came to ChemE expecting chemistry. I ended up studying systems.</h2>
    <p class="subline">What pulled me in was not just the material itself, but the process that puts it where it needs to go, in the right form, at the right time.</p>

    <div class="system-diagram reveal" aria-label="Droplet deposition process visual" style="--reveal-delay: 220ms">
      <div class="process-map" aria-label="Deposition input to process rule schematic">
        <div class="process-node input">
          <span>Input</span>
          <strong>IPA + microdevices</strong>
          <small>Suspended devices enter the deposition step.</small>
        </div>
        <span class="pm-arr" aria-hidden="true"></span>
        <div class="process-node transport">
          <span>Transport</span>
          <strong>Spreading · pinning · imbibition · drying</strong>
          <small>Boundary conditions determine contact-line motion.</small>
        </div>
        <span class="pm-arr" aria-hidden="true"></span>
        <div class="process-node output">
          <span>Output</span>
          <strong>Edge/center ratio + placement fidelity</strong>
          <small>The final pattern becomes a measurable response.</small>
        </div>
        <span class="pm-arr" aria-hidden="true"></span>
        <div class="process-node rule">
          <span>Rule</span>
          <strong>Substrate design criterion</strong>
          <small>Choose surfaces by the process window they create.</small>
        </div>
      </div>
      <div class="diagram-copy">
        <h3>From deposition behavior to an engineering rule.</h3>
        <p>Printed electronics sits at a manufacturing boundary I find exciting: devices too small to assemble by hand, workflows that do not fully exist yet, and process rules still open enough to shape. In deposition, the engineering problem is not just observing where microdevices land. It is building the measurement framework that turns the final pattern into a process rule.</p>
      </div>
    </div>
  </section>

  <section class="section reveal" aria-label="Process development loop" style="--reveal-delay: 240ms">
    <div class="eyebrow">My process-development loop</div>
    <h2>From observation to process rule.</h2>
    <p class="subline">Observe the phenomenon, isolate the control, measure the output, and convert the result into a decision another engineer could reproduce.</p>

    <div class="loop-grid reveal" style="--reveal-delay: 220ms">
      <article class="loop-step">
        <span class="loop-n">01</span>
        <h3>Observe</h3>
        <p>What is physically happening before the final structure locks in?</p>
        <span class="loop-example">Microdevices raft toward the droplet edge during drying</span>
      </article>
      <article class="loop-step">
        <span class="loop-n">02</span>
        <h3>Isolate</h3>
        <p>Which inputs can I actually control without changing the whole system?</p>
        <span class="loop-example">Porosity · wetting · backing condition · evaporation pathway</span>
      </article>
      <article class="loop-step">
        <span class="loop-n">03</span>
        <h3>Measure</h3>
        <p>What does better look like numerically, not just visually?</p>
        <span class="loop-example">Edge/center ratio · footprint evolution · repeatability metrics</span>
      </article>
      <article class="loop-step">
        <span class="loop-n">04</span>
        <h3>Decide</h3>
        <p>What should the next engineer or manufacturer do differently?</p>
        <span class="loop-example">Select boundary conditions that preserve placement fidelity</span>
      </article>
    </div>
  </section>

  <section class="section reveal" aria-label="Technical through-line" style="--reveal-delay: 280ms">
    <div class="eyebrow">The through-line</div>
    <h2>Systems built for transfer, not just demonstration.</h2>

    <div class="bridge-strip reveal" aria-label="Lab to deployment bridge" style="--reveal-delay: 200ms">
      <div class="bridge-step">
        <strong>Lab phenomena</strong>
        <span>Physical behavior appears under specific conditions.</span>
      </div>
      <div class="bridge-step">
        <strong>Process windows</strong>
        <span>Inputs and outputs become bounded, measured, and repeatable.</span>
      </div>
      <div class="bridge-step">
        <strong>Manufacturing rules</strong>
        <span>Another engineer can reproduce the method without guessing.</span>
      </div>
      <div class="bridge-step">
        <strong>Deployable systems</strong>
        <span>The technology holds under new surfaces, workflows, and use conditions.</span>
      </div>
    </div>

    <div class="open-question reveal" style="--reveal-delay: 240ms">
      <p class="q-label">A question that still bothers me</p>
      <p class="q-main">If substrate boundary conditions determine where microdevices land, what does the substrate-agnostic design rule look like?</p>
      <p class="q-body">I do not have the full answer yet, but I know what kind of answer would matter: a measurable process window another engineer could use. The work now is to connect droplet spreading, imbibition, pinning, and final device distribution into design rules that survive outside one lab setup — and eventually outside one research group.</p>
      <a class="q-link" href="{{ '/projects/micromodular-deposition/' | relative_url }}">Follow the current state of this work →</a>
    </div>

    <div class="timeline reveal" role="list" aria-label="Journey timeline" style="--reveal-delay: 260ms">
      <div class="time-step" role="listitem">
        <span class="time-dot"></span>
        <span class="time-place">Incheon</span>
        <span class="time-note">Origin</span>
      </div>
      <div class="time-step" role="listitem">
        <span class="time-dot"></span>
        <span class="time-place">Minnesota</span>
        <span class="time-note">The systems question forms</span>
      </div>
      <div class="time-step now" role="listitem">
        <span class="time-dot"></span>
        <span class="time-place">Georgia Tech</span>
        <span class="time-note">The answer takes shape</span>
      </div>
      <div class="time-step" role="listitem">
        <span class="time-dot"></span>
        <span class="time-place">Clean manufacturing</span>
        <span class="time-note">Technology that reaches people</span>
      </div>
    </div>

    <div class="cta-row">
      <a class="cta primary" href="{{ '/projects/' | relative_url }}">View process-development projects →</a>
      <a class="cta" href="{{ '/resume/' | relative_url }}">View résumé</a>
      <a class="cta" href="{{ '/contact/' | relative_url }}">Contact me</a>
    </div>
  </section>
</main>

<script>
  (function () {
    const page = document.querySelector('.bp.motion-enabled');
    if (!page) return;

    document.documentElement.classList.add('js');

    const revealItems = page.querySelectorAll('.reveal');
    if (!revealItems.length) return;

    if (!('IntersectionObserver' in window)) {
      revealItems.forEach((item) => item.classList.add('in-view'));
      return;
    }

    const observer = new IntersectionObserver((entries, obs) => {
      entries.forEach((entry) => {
        if (!entry.isIntersecting) return;
        entry.target.classList.add('in-view');
        obs.unobserve(entry.target);
      });
    }, {
      threshold: 0.12,
      rootMargin: '0px 0px -8% 0px'
    });

    revealItems.forEach((item, index) => {
      if (!item.style.getPropertyValue('--reveal-delay')) {
        item.style.setProperty('--reveal-delay', `${Math.min(index * 60, 240)}ms`);
      }
      observer.observe(item);
    });
  })();
</script>

