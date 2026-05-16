<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>PET-Xi | Day 1 Check-In</title>
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@700;800&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
:root{
  --pink:#D51A80;--pink-dark:#a01260;--pink-light:rgba(213,26,128,0.13);--pink-glow:rgba(213,26,128,0.28);
  --aqua:#44AFA1;--bg:#0f0f1a;--bg-card:rgba(255,255,255,0.045);--border:rgba(255,255,255,0.09);
  --text:#f0f0f8;--muted:rgba(240,240,248,0.48);--r:12px;
}
html,body{background:#0f0f1a !important;color:#f0f0f8 !important;min-height:100vh}
body{font-family:'DM Sans',sans-serif;overflow-x:hidden;position:relative}
body::before{content:'';position:fixed;inset:0;pointer-events:none;z-index:0;
  background:radial-gradient(ellipse 70% 50% at 0% 0%,rgba(213,26,128,0.18) 0%,transparent 60%),
  radial-gradient(ellipse 50% 40% at 100% 100%,rgba(68,175,161,0.1) 0%,transparent 55%)}
.wrap{position:relative;z-index:1;max-width:600px;margin:0 auto;padding:28px 20px 80px}
.hdr{display:flex;align-items:center;gap:13px;margin-bottom:40px;padding-bottom:22px;border-bottom:1px solid var(--border)}
.logo{width:44px;height:44px;background:var(--pink);border-radius:11px;display:flex;align-items:center;justify-content:center;font-family:'Syne',sans-serif;font-weight:800;font-size:16px;color:#fff;letter-spacing:-1px;flex-shrink:0;box-shadow:0 0 24px var(--pink-glow)}
.hdr h1{font-family:'Syne',sans-serif;font-size:14px;font-weight:700;letter-spacing:.03em;color:var(--text)}
.hdr p{font-size:12px;color:var(--muted);margin-top:2px}
.prog{margin-bottom:36px}
.prog-meta{display:flex;justify-content:space-between;margin-bottom:9px}
.prog-lbl{font-size:11px;font-weight:500;color:var(--muted);letter-spacing:.09em;text-transform:uppercase}
.prog-n{font-family:'Syne',sans-serif;font-size:12px;font-weight:700;color:var(--pink)}
.prog-track{height:2px;background:rgba(255,255,255,0.07);border-radius:99px;overflow:hidden}
.prog-fill{height:100%;background:linear-gradient(90deg,var(--pink),#ff6bb5);border-radius:99px;transition:width .45s cubic-bezier(.4,0,.2,1);box-shadow:0 0 8px var(--pink-glow)}
.card{animation:up .3s cubic-bezier(.4,0,.2,1) both}
@keyframes up{from{opacity:0;transform:translateY(16px)}to{opacity:1;transform:translateY(0)}}
.pill{display:inline-flex;background:var(--pink-light);border:1px solid rgba(213,26,128,.25);border-radius:99px;padding:3px 12px;font-size:10px;font-weight:600;color:var(--pink);letter-spacing:.08em;text-transform:uppercase;margin-bottom:16px}
.q-text{font-family:'Syne',sans-serif;font-size:21px;font-weight:700;line-height:1.3;margin-bottom:6px;letter-spacing:-.01em;color:var(--text)}
.q-sub{font-size:13px;color:var(--muted);margin-bottom:24px;line-height:1.55}
.opt{display:flex;align-items:center;gap:12px;padding:14px 16px;background:var(--bg-card);border:1.5px solid var(--border);border-radius:var(--r);cursor:pointer;transition:all .18s ease;width:100%;color:var(--text);font-family:'DM Sans',sans-serif;font-size:14px;position:relative;overflow:hidden;margin-bottom:9px;text-align:left}
.opt::after{content:'';position:absolute;inset:0;background:linear-gradient(135deg,var(--pink-light),transparent);opacity:0;transition:opacity .18s}
.opt:hover{border-color:rgba(213,26,128,.38);transform:translateX(3px)}
.opt:hover::after{opacity:1}
.opt.sel{border-color:var(--pink);background:var(--pink-light);box-shadow:0 0 0 1px var(--pink),0 3px 18px var(--pink-glow)}
.opt.sel::after{opacity:1}
.opt-label{flex:1;position:relative;z-index:1;line-height:1.4}
.dot{width:17px;height:17px;border-radius:50%;border:2px solid rgba(255,255,255,.18);flex-shrink:0;position:relative;z-index:1;display:flex;align-items:center;justify-content:center;font-size:9px;font-weight:700;color:#fff;transition:all .18s}
.opt.sel .dot{background:var(--pink);border-color:var(--pink);box-shadow:0 0 6px var(--pink-glow)}
.stars{display:flex;gap:8px;margin-bottom:8px}
.star{font-size:32px;cursor:pointer;transition:transform .12s,filter .12s;filter:grayscale(1) opacity(.22);user-select:none}
.star.lit{filter:none;transform:scale(1.08)}
.star-lbl{font-size:13px;color:var(--muted);min-height:18px;margin-bottom:20px}
textarea{width:100%;background:var(--bg-card);border:1.5px solid var(--border);border-radius:var(--r);padding:13px 15px;color:var(--text);font-family:'DM Sans',sans-serif;font-size:14px;line-height:1.5;resize:none;outline:none;transition:border-color .18s;display:block}
textarea:focus{border-color:rgba(213,26,128,.45)}
textarea::placeholder{color:var(--muted)}
.btags{margin:8px 0 18px}
.btag{display:inline-flex;align-items:center;gap:5px;padding:5px 12px;background:rgba(68,175,161,.1);border:1px solid rgba(68,175,161,.25);border-radius:99px;font-size:12px;color:var(--aqua);font-weight:500;margin:0 5px 6px 0}
.checks{display:grid;grid-template-columns:1fr 1fr;gap:8px;margin-bottom:4px}
.chk{display:flex;align-items:center;gap:9px;padding:10px 13px;background:var(--bg-card);border:1.5px solid var(--border);border-radius:var(--r);cursor:pointer;transition:all .18s;color:var(--text);font-size:13px;font-family:'DM Sans',sans-serif}
.chk:hover{border-color:rgba(213,26,128,.38)}
.chk.sel{border-color:var(--pink);background:var(--pink-light)}
.chk-box{width:15px;height:15px;border-radius:4px;border:2px solid rgba(255,255,255,.18);flex-shrink:0;display:flex;align-items:center;justify-content:center;font-size:8px;font-weight:700;color:#fff;transition:all .18s}
.chk.sel .chk-box{background:var(--pink);border-color:var(--pink)}
.yn{display:flex;gap:9px;margin-bottom:4px}
.yn-btn{flex:1;padding:13px;background:var(--bg-card);border:1.5px solid var(--border);border-radius:var(--r);cursor:pointer;text-align:center;font-family:'Syne',sans-serif;font-weight:700;font-size:14px;color:var(--muted);transition:all .18s}
.yn-btn:hover{border-color:rgba(213,26,128,.38);color:var(--text)}
.yn-btn.sel{border-color:var(--pink);background:var(--pink-light);color:var(--pink);box-shadow:0 0 0 1px var(--pink)}
.sub{margin-top:20px;padding-top:18px;border-top:1px solid var(--border)}
.sub-lbl{font-size:13px;color:var(--muted);margin-bottom:11px;font-weight:500}
.nav{display:flex;gap:10px;margin-top:32px}
.btn-back{padding:13px 20px;background:transparent;border:1.5px solid var(--border);border-radius:var(--r);color:var(--muted);font-family:'Syne',sans-serif;font-weight:600;font-size:13px;cursor:pointer;transition:all .18s}
.btn-back:hover{border-color:rgba(255,255,255,.18);color:var(--text)}
.btn-next{flex:1;padding:13px 24px;background:var(--pink);border:none;border-radius:var(--r);color:#fff;font-family:'Syne',sans-serif;font-weight:700;font-size:14px;cursor:pointer;transition:all .18s;box-shadow:0 4px 20px var(--pink-glow);letter-spacing:.01em}
.btn-next:hover{background:var(--pink-dark);transform:translateY(-1px);box-shadow:0 6px 24px var(--pink-glow)}
.btn-next:disabled{opacity:.32;cursor:not-allowed;transform:none;box-shadow:none}
.done{text-align:center;padding:48px 20px;animation:up .4s ease both}
.done-icon{font-size:56px;margin-bottom:22px;display:block}
.done h2{font-family:'Syne',sans-serif;font-size:26px;font-weight:800;margin-bottom:10px;color:var(--text)}
.done p{color:var(--muted);font-size:14px;line-height:1.65;max-width:340px;margin:0 auto}
.done-bar{width:64px;height:2px;background:var(--pink);border-radius:99px;margin:24px auto 0;box-shadow:0 0 10px var(--pink-glow)}
.err{font-size:12px;color:#ff6b6b;margin-top:8px;display:none}
</style>
</head>
<body>
<div class="wrap">
  <div class="hdr">
    <div class="logo">PX</div>
    <div>
      <h1>PET-Xi Training</h1>
      <p>Day 1 Check-In &mdash; about 3 minutes</p>
    </div>
  </div>
  <div class="prog">
    <div class="prog-meta">
      <span class="prog-lbl">Progress</span>
      <span class="prog-n" id="pn">1 of 8</span>
    </div>
    <div class="prog-track"><div class="prog-fill" id="pf" style="width:12.5%"></div></div>
  </div>
  <div id="survey"></div>
</div>

<script>
// ─── CONFIG ──────────────────────────────────────────────────────────────────
const LRS = "https://YOUR-AZURE-FUNCTION.azurewebsites.net/api/xapi";

// In production these come from the tokenised SMS link query params
const params = new URLSearchParams(window.location.search);
const ACTOR = {
  name: params.get("name") || "Learner",
  mbox: "mailto:" + (params.get("email") || "learner@petxi.co.uk")
};
const BARRIERS = (params.get("barriers") || "Mental health,Transport,Digital access").split(",");

// ─── xAPI ────────────────────────────────────────────────────────────────────
function send(verb, id, name, result) {
  const stmt = {
    actor: ACTOR,
    verb: { id: "http://adlnet.gov/expapi/verbs/" + verb, display: { "en-GB": verb } },
    object: { id: "https://petxi.co.uk/survey/day1/" + id, definition: { name: { "en-GB": name } } },
    result: result || {},
    timestamp: new Date().toISOString(),
    context: { platform: "PET-Xi Day 1 Survey" }
  };
  return fetch(LRS, {
    method: "POST",
    headers: { "Content-Type": "application/json" },
    body: JSON.stringify(stmt)
  }).catch(e => console.warn("xAPI send failed:", e));
}

// ─── STATE ───────────────────────────────────────────────────────────────────
let cur = 0;
const ans = {};

const SECS = ["Today's Training","Today's Training","Today's Training",
              "Your Needs","Your Needs","Support","Support","Anything Else"];

const QS = [
  { id:"rating",        type:"stars",    req:true,
    text:"How was today's session?",
    sub:"Your honest first impression — no wrong answers." },
  { id:"worked",        type:"text",     req:false,
    text:"What worked well for you today?",
    sub:"Even one thing helps us understand what's landing.",
    ph:"e.g. The trainer explained things clearly, I liked the group work..." },
  { id:"better",        type:"text",     req:false,
    text:"What could have been better?",
    sub:"Be straight with us.",
    ph:"e.g. Too much sitting, would have liked more breaks..." },
  { id:"barriers",      type:"barriers", req:true,
    text:"Are these still your current needs?",
    sub:"We have these on record from your enrolment. Let us know if anything has changed." },
  { id:"barriers_more", type:"text",     req:false,
    text:"Anything else we should know about your situation right now?",
    sub:"Optional — only share what you're comfortable with.",
    ph:"e.g. I'm going through a difficult time at home at the moment..." },
  { id:"trainer_talk",  type:"trainer",  req:true,
    text:"Did you get to talk with your trainer about any needs or concerns today?",
    sub:null },
  { id:"support_cats",  type:"checks",   req:false,
    text:"Is there anything you need help with?",
    sub:"Tick everything that applies — this goes straight to our support team." },
  { id:"escalation",    type:"escalate", req:false,
    text:"Anything you'd like to raise directly with PET-Xi?",
    sub:"Not your trainer — someone from our wider team. Goes to the right person." }
];

// ─── RENDER ──────────────────────────────────────────────────────────────────
function render() {
  const q = QS[cur];
  document.getElementById("pn").textContent = (cur+1) + " of " + QS.length;
  document.getElementById("pf").style.width = ((cur+1)/QS.length*100).toFixed(1) + "%";

  let h = `<div class="card"><div class="pill">${SECS[cur]}</div>
    <div class="q-text">${q.text}</div>
    ${q.sub ? `<div class="q-sub">${q.sub}</div>` : ""}`;

  if (q.type === "stars") {
    const v = ans.rating || 0;
    const lbls = ["","Really struggled","Wasn't great","It was okay","Pretty good","Excellent"];
    h += `<div class="stars" id="stars">`;
    for (let i=1;i<=5;i++) h += `<span class="star${i<=v?' lit':''}" data-v="${i}">★</span>`;
    h += `</div><div class="star-lbl" id="slbl">${v?lbls[v]:""}</div>`;
  }

  if (q.type === "text") {
    h += `<textarea id="ta" rows="4" placeholder="${q.ph||''}">${ans[q.id]||""}</textarea>`;
  }

  if (q.type === "barriers") {
    h += `<div class="btags">`;
    BARRIERS.forEach(b => h += `<span class="btag">✦ ${b.trim()}</span>`);
    h += `</div>`;
    const v = ans.barriers;
    [["yes","✓","Yes, that's still accurate"],
     ["partly","◎","Partly — something has changed"],
     ["no","✕","No — these are out of date"]].forEach(([val,icon,lbl]) => {
      h += `<div class="opt${v===val?' sel':''}" data-v="${val}" onclick="pickOpt(this,'barriers')">
        <span class="opt-label">${icon} ${lbl}</span><span class="dot">${v===val?'✓':''}</span></div>`;
    });
    if (v==="partly"||v==="no") {
      h += `<div style="margin-top:14px"><textarea id="bdet" rows="3"
        placeholder="What's changed?">${ans.barriers_detail||""}</textarea></div>`;
    }
  }

  if (q.type === "trainer") {
    const v = ans.trainer_talk, fv = ans.trainer_followup;
    [["yes","Yes, we talked"],["partly","Briefly / partly"],["no","No, we didn't"]].forEach(([val,lbl])=>{
      h += `<div class="opt${v===val?' sel':''}" data-v="${val}"
        onclick="pickOpt(this,'trainer_talk');rerender()">
        <span class="opt-label">${lbl}</span><span class="dot">${v===val?'✓':''}</span></div>`;
    });
    if (v==="partly"||v==="no") {
      h += `<div class="sub"><div class="sub-lbl">Would you like someone from PET-Xi to follow this up with you?</div>
        <div class="yn">
          <div class="yn-btn${fv==='yes'?' sel':''}" onclick="pickYN(this,'trainer_followup','yes')">Yes please</div>
          <div class="yn-btn${fv==='no'?' sel':''}" onclick="pickYN(this,'trainer_followup','no')">No, I'm fine</div>
        </div></div>`;
    }
  }

  if (q.type === "checks") {
    const v = ans.support_cats || [];
    const opts = [["🧒","Childcare"],["🚌","Transport"],["🏠","Housing"],["💻","Digital access"],
                  ["🧠","Mental health"],["💷","Financial"],["📖","English / language"],["♿","Health / disability"]];
    h += `<div class="checks">`;
    opts.forEach(([icon,lbl]) => {
      const s = v.includes(lbl);
      h += `<div class="chk${s?' sel':''}" onclick="togChk(this,'support_cats','${lbl}')">
        <div class="chk-box">${s?'✓':''}</div>${icon} ${lbl}</div>`;
    });
    h += `</div>`;
  }

  if (q.type === "escalate") {
    const v = ans.escalation;
    h += `<div class="yn">
      <div class="yn-btn${v==='yes'?' sel':''}" onclick="pickYN(this,'escalation','yes');rerender()">Yes, I do</div>
      <div class="yn-btn${v==='no'?' sel':''}" onclick="pickYN(this,'escalation','no');rerender()">No, I'm good</div>
    </div>`;
    if (v==="yes") {
      h += `<div style="margin-top:14px"><textarea id="esct" rows="4"
        placeholder="Tell us what's on your mind — this goes to the right person...">${ans.escalation_detail||""}</textarea></div>`;
    }
  }

  const ok = canGo(q);
  h += `<div class="nav">
    ${cur>0?`<button class="btn-back" onclick="goBack()">← Back</button>`:""}
    <button class="btn-next" id="bn" onclick="goNext()" ${ok?"":"disabled"}>
      ${cur===QS.length-1?"Submit check-in ✓":"Continue →"}
    </button>
  </div></div>`;

  document.getElementById("survey").innerHTML = h;
  bind(q);
}

function canGo(q) {
  if (!q.req) return true;
  if (q.type==="stars") return (ans.rating||0)>0;
  if (q.type==="barriers") return !!ans.barriers;
  if (q.type==="trainer") return !!ans.trainer_talk;
  return true;
}

function bind(q) {
  if (q.type==="stars") {
    document.querySelectorAll(".star").forEach(s => s.addEventListener("click", () => {
      const v = parseInt(s.dataset.v);
      ans.rating = v;
      document.querySelectorAll(".star").forEach((st,i) => st.classList.toggle("lit",i<v));
      const lbls=["","Really struggled","Wasn't great","It was okay","Pretty good","Excellent"];
      document.getElementById("slbl").textContent = lbls[v];
      document.getElementById("bn").disabled = false;
    }));
  }
  const ta = document.getElementById("ta");
  if (ta) ta.addEventListener("input", () => { ans[q.id] = ta.value; });
  const bdet = document.getElementById("bdet");
  if (bdet) bdet.addEventListener("input", () => { ans.barriers_detail = bdet.value; });
  const esct = document.getElementById("esct");
  if (esct) esct.addEventListener("input", () => { ans.escalation_detail = esct.value; });
}

function pickOpt(el, key) {
  ans[key] = el.dataset.v;
  document.getElementById("bn").disabled = false;
}

function pickYN(el, key, val) {
  ans[key] = val;
  el.parentElement.querySelectorAll(".yn-btn").forEach(b => b.classList.remove("sel"));
  el.classList.add("sel");
}

function togChk(el, key, val) {
  if (!ans[key]) ans[key] = [];
  const i = ans[key].indexOf(val);
  if (i>-1) ans[key].splice(i,1); else ans[key].push(val);
  el.classList.toggle("sel", ans[key].includes(val));
  el.querySelector(".chk-box").textContent = ans[key].includes(val) ? "✓" : "";
}

function rerender() { render(); }

function goBack() {
  if (cur>0) { cur--; render(); window.scrollTo(0,0); }
}

function goNext() {
  const q = QS[cur];
  const ta = document.getElementById("ta");
  if (ta) ans[q.id] = ta.value;
  send("answered", q.id, q.text, { response: JSON.stringify(ans[q.id]||"") });
  if (cur < QS.length-1) { cur++; render(); window.scrollTo(0,0); }
  else { submit(); }
}

function submit() {
  const tier = getTier();
  send("completed", "day1-survey", "PET-Xi Day 1 Check-In", {
    completion: true,
    response: JSON.stringify({ ...ans, alert_tier: tier })
  });
  document.getElementById("survey").innerHTML = `
    <div class="done">
      <span class="done-icon">✓</span>
      <h2>Thank you — that's really helpful.</h2>
      <p>We've received your check-in. If you asked for a follow-up, someone from PET-Xi will be in touch shortly.</p>
      <div class="done-bar"></div>
    </div>`;
  document.getElementById("pf").style.width = "100%";
  document.getElementById("pn").textContent = "Complete";
}

function getTier() {
  const red = ["safe","harm","hurt","abuse","crisis","emergency","scared","danger","suicid","threat"];
  const etxt = (ans.escalation_detail||"").toLowerCase();
  if (red.some(k=>etxt.includes(k)) || (ans.escalation==="yes"&&(ans.rating||5)<=2)) return "red";
  if (ans.escalation==="yes"||ans.trainer_followup==="yes"||
      ans.barriers==="no"||ans.barriers==="partly"||(ans.rating||5)<=2) return "amber";
  return "green";
}

send("launched","day1-survey","PET-Xi Day 1 Check-In");
render();
</script>
</body>
</html>
