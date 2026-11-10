<!DOCTYPE html>
<html lang="en"><head><meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Sahana Shetty — Portfolio</title>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;500;700&family=JetBrains+Mono:wght@400&display=swap">
<style>
:root{color-scheme:dark;--bg:#05070d;--ch:#0e131f;--navy:#0a1630;--blue:#3b82f6;--cy:#22d3ee;--tx:#e6ebf5;--mu:#8b97ad;--ln:#1e2a42;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
*{box-sizing:border-box}html{scroll-behavior:smooth;scroll-padding-top:70px}
body{margin:0;background:var(--bg);color:var(--tx);font:16px/1.6 "Space Grotesk",system-ui,sans-serif;overflow-x:hidden}
a{color:inherit}.mono{font-family:"JetBrains Mono",ui-monospace,monospace}
nav{position:fixed;top:env(safe-area-inset-top,0px);left:0;right:0;z-index:50;display:flex;justify-content:space-between;align-items:center;padding:14px 5vw;background:rgba(5,7,13,.7);backdrop-filter:blur(12px);border-bottom:1px solid var(--ln)}
nav b{letter-spacing:.12em;font-weight:500}nav div{display:flex;gap:18px;font-size:13px;color:var(--mu);overflow-x:auto}nav a{text-decoration:none;white-space:nowrap}nav a:hover,nav a:focus-visible{color:var(--cy);outline:none}
section{padding:110px 6vw;max-width:1200px;margin:auto;position:relative}
h2{font-size:clamp(28px,5vw,48px);font-weight:300;margin:0 0 8px;letter-spacing:-.02em}
.eyebrow{font:12px "JetBrains Mono",monospace;color:var(--cy);letter-spacing:.2em;text-transform:uppercase}
.rv{opacity:0;transform:translateY(30px);transition:1s cubic-bezier(.2,.7,.2,1)}.rv.in{opacity:1;transform:none}
#hero{max-width:none;min-height:100vh;display:flex;flex-direction:column;justify-content:center;padding-left:8vw;overflow:hidden;background:radial-gradient(ellipse at 75% 30%,#0f2a5c55,transparent 60%),radial-gradient(ellipse at 20% 90%,#0a3a4a44,transparent 55%)}
#cv{position:absolute;inset:0;width:100%;height:100%}
#hero>*:not(canvas){position:relative;max-width:820px}
h1{font-size:clamp(44px,9vw,112px);line-height:.95;font-weight:700;margin:14px 0;letter-spacing:-.04em;background:linear-gradient(120deg,#fff 30%,var(--cy));-webkit-background-clip:text;background-clip:text;color:transparent}
.role{color:var(--cy);font-size:clamp(13px,2vw,17px)}.lead{color:var(--mu);font-size:clamp(16px,2vw,20px);max-width:600px}
.cta{display:flex;gap:14px;flex-wrap:wrap;margin-top:26px}
.btn{padding:13px 26px;border-radius:99px;border:1px solid var(--blue);text-decoration:none;font-size:14px;transition:.3s}
.btn.p{background:var(--blue);color:#fff}.btn:hover,.btn:focus-visible{box-shadow:0 0 28px #3b82f666;transform:translateY(-2px);outline:none}
.hero-in{animation:up 1.2s both}@keyframes up{from{opacity:0;transform:translateY(40px)}}
.cols{display:grid;grid-template-columns:1.1fr 1fr;gap:6vw}
.big{font-size:clamp(22px,3vw,34px);font-weight:300;line-height:1.35}.big em{font-style:normal;color:var(--cy)}
.stat{display:flex;gap:30px;margin-top:24px}.stat div{border-left:2px solid var(--blue);padding-left:14px}.stat b{display:block;font-size:30px;font-weight:500}.stat span{color:var(--mu);font-size:13px}
.p-mu{color:var(--mu)}
/* skills */
#uni{display:grid;grid-template-columns:260px 1fr;gap:30px;margin-top:30px;align-items:center}
.cats{display:flex;flex-direction:column;gap:10px}
.cat{background:var(--ch);border:1px solid var(--ln);color:var(--tx);padding:14px 18px;border-radius:12px;text-align:left;font:inherit;cursor:pointer;transition:.3s}
.cat[aria-selected=true],.cat:hover{border-color:var(--cy);box-shadow:0 0 24px #22d3ee22 inset}
.field{position:relative;min-height:380px;border:1px solid var(--ln);border-radius:20px;background:radial-gradient(circle at 50% 50%,#0b1c3d,#070b14);overflow:hidden}
.field svg{position:absolute;inset:0;width:100%;height:100%}
.core{position:absolute;left:50%;top:50%;transform:translate(-50%,-50%);width:92px;height:92px;border-radius:50%;display:grid;place-items:center;text-align:center;font-size:12px;border:1px solid var(--cy);box-shadow:0 0 40px #22d3ee44;background:#06101f}
.chip{position:absolute;padding:8px 16px;border-radius:99px;background:#0d1d3acc;border:1px solid #2b4a8a;font-size:14px;animation:fl 5s ease-in-out infinite alternate;cursor:default;transition:.3s;transform:translate(-50%,-50%)}
.chip:hover{border-color:var(--cy);color:var(--cy)}@keyframes fl{to{margin-top:-14px}}
/* book */
#books{padding-bottom:120px;max-width:1400px}
.stage{perspective:2600px;height:min(82vw,780px);display:flex;justify-content:center;align-items:center;margin-top:24px;touch-action:pan-y;user-select:none}
.book{--pw:min(460px,43vw);--ph:min(640px,62vw);position:relative;width:var(--pw);height:var(--ph);transform-style:preserve-3d;transition:transform 1s cubic-bezier(.645,.045,.355,1);filter:drop-shadow(0 50px 50px #000c);cursor:grab}
.leaf{position:absolute;inset:0;transform-origin:left center;transform-style:preserve-3d;transition:transform 1.1s cubic-bezier(.645,.045,.355,1)}
.leaf.f{transform:rotateY(-180deg)}
.face{position:absolute;inset:0;backface-visibility:hidden;-webkit-backface-visibility:hidden;overflow:hidden;background:#eef2fa;color:#141b2d;font-size:clamp(9px,1.1vw,14px);line-height:1.45;border-radius:2px 8px 8px 2px;box-shadow:1px 0 0 #c7cee0,2px 0 0 #b3bcd4,3px 0 0 #9ea8c4,4px 0 0 #8893b0,5px 0 0 #6f7a99;display:flex;flex-direction:column}
.face.b{transform:rotateY(180deg);border-radius:8px 2px 2px 8px;box-shadow:-1px 0 0 #c7cee0,-2px 0 0 #b3bcd4,-3px 0 0 #9ea8c4,-4px 0 0 #8893b0}
.face::before{content:"";position:absolute;inset:0;pointer-events:none;z-index:6;background:linear-gradient(90deg,#0005,#0000 8%,#0000 93%,#0002)}
.pad{padding:8% 8% 9%;display:flex;flex-direction:column;gap:2.6%;height:100%;position:relative}
.num{position:absolute;top:2%;right:7%;font:700 6.5em/1 "Space Grotesk",sans-serif;letter-spacing:-.06em;color:#2457c5;opacity:.12;pointer-events:none}
.face h3{margin:0;font-size:1.75em;line-height:1.05;letter-spacing:-.02em;font-weight:700}.face h4{margin:4px 0 0;font:500 .78em "JetBrains Mono",monospace;letter-spacing:.14em;text-transform:uppercase;color:#2457c5}.face p{margin:0}.face ul{margin:0;padding-left:1.1em}
.face .eyebrow{color:#2457c5;font-size:.8em}
.face figure{margin:0}.z{cursor:zoom-in}.face figure svg{width:100%;height:auto;display:block;border-radius:8px;border:1px solid #c5cde0}
figcaption{font-size:.8em;color:#4b5873;margin-top:4px;display:flex;gap:6px;align-items:flex-start}
.tg{font:.7em "JetBrains Mono",monospace;padding:1px 7px;border-radius:99px;background:#dbe5fb;color:#1e3f8f;white-space:nowrap}.tg.w{background:#fdecc8;color:#8a5a00}
.bd{display:flex;flex-wrap:wrap;gap:5px}.bd span{display:flex;align-items:center;gap:5px;border:1px solid #c5cde0;background:#fff;border-radius:8px;padding:3px 9px;font-weight:500}.bd i{width:8px;height:8px;border-radius:2px}
.stats{display:grid;grid-template-columns:repeat(3,1fr);gap:6px}.stats div{background:#fff;border:1px solid #c5cde0;border-radius:10px;padding:8px}.stats b{display:block;font-size:1.5em;line-height:1.1}.stats small{color:#58689a}
.two{display:grid;grid-template-columns:1fr 1fr;gap:8px}.two>div{display:flex;flex-direction:column;gap:5px}
.cov{position:relative;color:#fff;justify-content:flex-end;background:#06122b}.cov .bg{position:absolute;inset:0;width:100%;height:100%}.cov .ov{position:absolute;inset:0;background:linear-gradient(180deg,#0000 25%,#050b1af0)}.cov .tx{position:relative;padding:9%}.cov h3{font-size:2.3em}.cov .eyebrow{color:#67e8f9}.cov p{opacity:.8;margin-top:6px}
.dk{background:linear-gradient(160deg,#06122b,#0b2250);color:#e6ebf5}.dk .eyebrow{color:#67e8f9}
.pn{position:absolute;bottom:2.4%;font:.7em "JetBrains Mono",monospace;color:#7a869f;z-index:7}.pn.l{left:8%}.pn.r{right:8%}.dk .pn,.cov .pn{color:#ffffff99}
.toc{display:flex;flex-direction:column;gap:8px}.toc button{all:unset;cursor:pointer;display:flex;gap:10px;align-items:center;background:#fff;border:1px solid #c5cde0;border-radius:10px;padding:6px;font-weight:500}.toc button:hover,.toc button:focus-visible{border-color:#2457c5}.toc .th{width:22%;flex:none}.toc svg{display:block;width:100%;border-radius:6px}.toc b{color:#2457c5;font-family:"JetBrains Mono",monospace}
.ctl{display:flex;justify-content:center;gap:12px;flex-wrap:wrap;margin-top:14px}.ctl button{background:var(--ch);color:var(--tx);border:1px solid var(--ln);border-radius:99px;padding:10px 22px;font:inherit;cursor:pointer;transition:.3s}.ctl button:hover:not(:disabled){border-color:var(--cy)}.ctl button:disabled{opacity:.35;cursor:default}
.prog{height:3px;background:var(--ln);border-radius:9px;max-width:420px;margin:16px auto 8px;overflow:hidden}.prog i{display:block;height:100%;width:0;background:linear-gradient(90deg,var(--blue),var(--cy));transition:width 1s}
#lb{position:fixed;inset:0;z-index:100;background:#000d;display:grid;place-items:center;padding:5vw;text-align:center}#lb[hidden]{display:none}#lbc svg{width:min(92vw,900px);max-height:78vh;border-radius:12px;background:#fff}#lbc p{color:var(--mu);margin:10px 0 0;font-size:13px}#lbx{position:absolute;top:calc(14px + env(safe-area-inset-top,0px));right:18px;background:var(--ch);color:var(--tx);border:1px solid var(--ln);border-radius:99px;width:42px;height:42px;font-size:18px;cursor:pointer}
/* gallery */
.gal{display:grid;grid-template-columns:repeat(auto-fill,minmax(250px,1fr));gap:22px;margin-top:34px;perspective:1000px}
.ex{background:linear-gradient(160deg,#101a2e,#0a0f1b);border:1px solid var(--ln);border-radius:16px;padding:24px;min-height:190px;transition:transform .2s,border-color .3s;transform-style:preserve-3d;position:relative}
.ex:hover{border-color:var(--blue)}.ex small{font:11px "JetBrains Mono",monospace;color:var(--cy);letter-spacing:.15em}.ex h3{margin:10px 0 6px;font-weight:500;font-size:19px}.ex p{margin:0;color:var(--mu);font-size:14px}.ex.ph2{border-style:dashed;opacity:.75}
/* terminal */
.term{margin-top:30px;background:#060a12;border:1px solid var(--ln);border-radius:14px;overflow:hidden;max-width:720px}
.term header{display:flex;gap:7px;padding:12px 16px;border-bottom:1px solid var(--ln)}.term header i{width:11px;height:11px;border-radius:50%;background:#26334f}
.term pre{margin:0;padding:22px;font:14px/1.9 "JetBrains Mono",monospace;white-space:pre-wrap;min-height:210px}
.term a{color:var(--cy);text-decoration:none;border-bottom:1px dashed var(--cy)}.term a:hover{background:#22d3ee22}.cur{display:inline-block;width:8px;height:15px;background:var(--cy);animation:bl 1s steps(1) infinite;vertical-align:-2px}@keyframes bl{50%{opacity:0}}
footer{text-align:center;color:var(--mu);font-size:13px;padding:40px}
@media(max-width:800px){.cols,#uni{grid-template-columns:1fr}.book{--pw:46vw;--ph:68vw}.stage{height:98vw}}
@media(prefers-reduced-motion:reduce){*{animation:none!important;transition-duration:.01s!important}}
</style></head><body>
<nav><b>SS</b><div><a href="#about">About</a><a href="#skills">Skills</a><a href="#books">Projects</a><a href="#gallery">Achievements</a><a href="#contact">Contact</a></div></nav>

<header id="hero"><canvas id="cv" aria-hidden="true"></canvas>
<div class="eyebrow hero-in">Bengaluru · Class of 2026</div>
<h1 class="hero-in" style="animation-delay:.2s">Sahana<br>Shetty</h1>
<div class="role mono hero-in" style="animation-delay:.4s">Software Engineer | AI &amp; ML Enthusiast | GenAI Developer</div>
<p class="lead hero-in" style="animation-delay:.6s">I turn messy, real-world problems into working systems — from pixel-level deep learning to full-stack products.</p>
<div class="cta hero-in" style="animation-delay:.8s"><a class="btn p" href="#books">Explore My Work</a><a class="btn" href="#contact">Contact Me</a></div></header>

<section id="about"><div class="eyebrow rv">01 — About</div>
<div class="cols"><div class="big rv">I’m a <em>2026 B.Tech Information Technology</em> graduate who likes understanding how things work — then building them <em>end to end</em>.</div>
<div class="rv"><p class="p-mu">My interests sit across software engineering, AI/ML and Generative AI. I learn by building: picking a real problem, shipping a first version, and iterating on what breaks. That’s how I’ve worked on aerial-imagery segmentation, computer-vision attendance, and RAG-based assistants.</p>
<div class="stat"><div><b>9.16</b><span>CGPA / 10</span></div><div><b>3</b><span>hackathons</span></div><div><b>CMRU</b><span>Chancellor’s List</span></div></div></div></div></section>

<section id="skills"><div class="eyebrow rv">02 — Skills</div><h2 class="rv">Technology universe</h2><p class="p-mu rv">Choose a constellation to explore.</p>
<div id="uni" class="rv"><div class="cats" role="tablist" aria-label="Skill categories" id="cats"></div><div class="field" id="field" aria-live="polite"><svg id="lines"></svg><div class="core mono" id="core"></div></div></div></section>

<section id="books"><div class="eyebrow rv">03 — Projects</div><h2 class="rv">The book of builds</h2><p class="p-mu rv">Drag, swipe, use ← → keys or the buttons — and tap any figure to enlarge it.</p>
<div class="stage" id="stage"><div class="book" id="book" aria-label="Interactive project book"></div></div>
<div class="ctl"><button id="prev">← Previous</button><button id="toc">Contents</button><button id="next">Next →</button></div><div class="prog" aria-hidden="true"><i id="pb"></i></div><p class="mono p-mu" id="pg" style="text-align:center;font-size:13px"></p></section>

<section id="gallery"><div class="eyebrow rv">04 — Achievements</div><h2 class="rv">Digital gallery</h2>
<div class="gal" id="gal"></div></section>

<section id="contact"><div class="eyebrow rv">05 — Contact</div><h2 class="rv">Open a connection</h2>
<div class="term rv"><header><i></i><i></i><i></i></header><pre id="tm" aria-live="polite"></pre></div></section>
<footer>© 2026 Sahana Shetty</footer>

<div id="lb" hidden role="dialog" aria-modal="true" aria-label="Enlarged figure"><button id="lbx" aria-label="Close">✕</button><div id="lbc"></div></div>
<script>
// ---- CONFIG: edit these ----
const LINKS={github:"https://github.com/sahanashettygithub",linkedin:"https://www.linkedin.com/in/YOUR-LINKEDIN",email:"mailto:YOUR-EMAIL@example.com"};
const $=s=>document.querySelector(s),reduce=matchMedia("(prefers-reduced-motion:reduce)").matches;
// reveal
const io=new IntersectionObserver(e=>e.forEach(x=>x.isIntersecting&&x.target.classList.add("in")),{threshold:.15});document.querySelectorAll(".rv").forEach(n=>io.observe(n));
// particles
(()=>{const c=$("#cv"),x=c.getContext("2d");let w,h,P=[];const r=()=>{w=c.width=c.offsetWidth;h=c.height=c.offsetHeight;P=Array.from({length:Math.min(70,w/18|0)},()=>({x:Math.random()*w,y:Math.random()*h,vx:(Math.random()-.5)*.3,vy:(Math.random()-.5)*.3}))};r();addEventListener("resize",r);
const f=()=>{x.clearRect(0,0,w,h);P.forEach((p,i)=>{if(!reduce){p.x=(p.x+p.vx+w)%w;p.y=(p.y+p.vy+h)%h}x.fillStyle="#22d3ee99";x.fillRect(p.x,p.y,1.6,1.6);for(let j=i+1;j<P.length;j++){const q=P[j],d=Math.hypot(p.x-q.x,p.y-q.y);if(d<120){x.strokeStyle=`rgba(59,130,246,${.18*(1-d/120)})`;x.beginPath();x.moveTo(p.x,p.y);x.lineTo(q.x,q.y);x.stroke()}}});requestAnimationFrame(f)};f()})();
// skills
const SK={"Programming":["Python","SQL","JavaScript"],"Data & AI":["Pandas","NumPy","Deep Learning","Computer Vision"],"Generative AI":["RAG","LangChain","ChromaDB","LLM APIs"],"Frameworks":["Flask","Streamlit","Gradio"],"Tools & Platforms":["Git","GitHub","Azure AI Services","n8n"]};
(()=>{const cats=$("#cats"),field=$("#field"),lines=$("#lines");
function show(k){cats.querySelectorAll("button").forEach(b=>b.setAttribute("aria-selected",b.dataset.k==k));$("#core").textContent=k;field.querySelectorAll(".chip").forEach(n=>n.remove());lines.innerHTML="";const L=SK[k],W=field.clientWidth,H=field.clientHeight;
L.forEach((s,i)=>{const a=i/L.length*Math.PI*2-Math.PI/2,px=50+Math.cos(a)*34,py=50+Math.sin(a)*34;const ln=document.createElementNS("http://www.w3.org/2000/svg","line");ln.setAttribute("x1","50%");ln.setAttribute("y1","50%");ln.setAttribute("x2",px+"%");ln.setAttribute("y2",py+"%");ln.setAttribute("stroke","#3b82f6");ln.setAttribute("stroke-opacity",".45");lines.appendChild(ln);
const c=document.createElement("div");c.className="chip";c.textContent=s;c.style.left=px+"%";c.style.top=py+"%";c.style.animationDelay=i*.6+"s";field.appendChild(c)})}
Object.keys(SK).forEach((k,i)=>{const b=document.createElement("button");b.className="cat";b.role="tab";b.dataset.k=k;b.innerHTML=`<span class="mono p-mu">0${i+1}</span> ${k}`;b.onclick=()=>show(k);cats.appendChild(b)});show("Generative AI")})();
// book
(()=>{
const CL=[["Water","#2f6fdb","#1d4f7a"],["Forest","#2e9e5b","#2a5a36"],["Cropland","#e0b341","#8c8a47"],["Urban","#8a93a6","#6c7078"],["Barren","#b9764a","#7d6246"]];
const cls=(x,y,s)=>{const v=Math.sin(x*.55+s)+Math.cos(y*.5+s*.7)+Math.sin((x+y)*.3+s*2);return v<-1.1?0:v<-.2?1:v<.6?2:v<1.2?3:4};
function aer(s,m){let r="";for(let y=0;y<20;y++)for(let x=0;x<16;x++){const c=cls(x,y,s);r+=`<rect x="${x*10}" y="${y*10}" width="10.5" height="10.5" fill="${CL[c][m?1:2]}"${m?"":` opacity="${.82+((x*7+y*13)%5)/28}"`}/>`}
return `<svg viewBox="0 0 160 200" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Illustrative ${m?"segmentation mask":"aerial view"}"><defs><filter id="bl"><feGaussianBlur stdDeviation="1.6"/></filter></defs>${m?r:`<g filter="url(#bl)">${r}</g><path d="M0 100Q80 60 160 120" stroke="#d8d2c0" stroke-width="2" fill="none" opacity=".7"/>`}</svg>`}
const bg=s=>s.replace("<svg ",'<svg class="bg" preserveAspectRatio="xMidYMid slice" ');
const MK='<defs><marker id="ar" markerWidth="6" markerHeight="6" refX="3" refY="3" orient="auto"><path d="M0 0L6 3L0 6z" fill="#2457c5"/></marker></defs>';
const fig=(svg,cap,t="ILLUSTRATIVE",w="")=>`<figure class="z" tabindex="0" role="button" aria-label="Enlarge: ${cap}">${svg}<figcaption><span class="tg ${w}">${t}</span>${cap}</figcaption></figure>`;
const ph=l=>fig(`<svg viewBox="0 0 200 120" xmlns="http://www.w3.org/2000/svg"><rect width="200" height="120" fill="#fff8e8"/><rect x="6" y="6" width="188" height="108" rx="8" fill="none" stroke="#c28a1a" stroke-dasharray="5 4"/><text x="100" y="58" text-anchor="middle" font-size="10" fill="#8a5a00" font-family="monospace">${l}</text><text x="100" y="74" text-anchor="middle" font-size="7" fill="#8a5a00" font-family="monospace">replace with your real screenshot</text></svg>`,l,"PLACEHOLDER","w");
const bd=a=>`<div class="bd">${a.map(([n,c])=>`<span><i style="background:${c}"></i>${n}</span>`).join("")}</div>`;
const bx=(x,y,w,h,t,s,f="#dbe5fb",st="#2457c5")=>`<rect x="${x}" y="${y}" width="${w}" height="${h}" rx="8" fill="${f}" stroke="${st}"/><text x="${x+w/2}" y="${y+h/2-(s?1:-4)}" text-anchor="middle" font-size="11" font-weight="700" fill="#141b2d">${t}</text>${s?`<text x="${x+w/2}" y="${y+h/2+11}" text-anchor="middle" font-size="8" fill="#58689a">${s}</text>`:""}`;
const arw=(x,a,b)=>`<line x1="${x}" y1="${a}" x2="${x}" y2="${b}" stroke="#2457c5" stroke-width="1.5" marker-end="url(#ar)"/>`;
const pipe=()=>`<svg viewBox="0 0 220 340" xmlns="http://www.w3.org/2000/svg" font-family="Space Grotesk,sans-serif">${MK}<rect width="220" height="340" fill="#f4f7ff"/>${bx(45,8,130,44,"Aerial image","input")}${arw(110,52,76)}<rect x="12" y="78" width="196" height="186" rx="12" fill="#fff" stroke="#2457c5" stroke-dasharray="4 3"/><text x="110" y="95" text-anchor="middle" font-size="10" font-weight="700" fill="#2457c5">DeepLabV3+</text>${bx(28,104,164,40,"ResNet-50","encoder backbone")}${arw(110,144,156)}${bx(28,158,164,40,"ASPP","multi-scale context")}${arw(110,198,210)}${bx(28,212,164,40,"Decoder","boundary refinement")}${arw(110,264,286)}${bx(45,288,130,44,"Segmentation mask","class per pixel","#dff3e8","#0e9f6e")}</svg>`;
const ic=(k,y)=>({c:`<rect x="20" y="${y+23}" width="20" height="14" rx="3"/><circle cx="30" cy="${y+30}" r="4"/>`,d:`<rect x="20" y="${y+20}" width="20" height="20" stroke-dasharray="3 2"/><circle cx="30" cy="${y+28}" r="4"/>`,r:`<circle cx="30" cy="${y+26}" r="5"/><path d="M21 ${y+40}q9-9 18 0"/>`,a:`<path d="M22 ${y+24}h16M22 ${y+30}h16M22 ${y+36}h10"/>`})[k];
const flow=()=>{const S=[["c","Camera input","live frame / image"],["d","Face detection","OpenCV, custom-trained"],["r","Recognition","match against known faces"],["a","Attendance record","saved via Flask app"]];return `<svg viewBox="0 0 230 290" xmlns="http://www.w3.org/2000/svg" font-family="Space Grotesk,sans-serif">${MK}<rect width="230" height="290" fill="#f4f7ff"/>${S.map((s,i)=>{const y=i*70+5;return `<circle cx="30" cy="${y+30}" r="22" fill="#dbe5fb"/><g stroke="#2457c5" fill="none" stroke-width="1.6">${ic(s[0],y)}</g><text x="64" y="${y+28}" font-size="12" font-weight="700" fill="#141b2d">${s[1]}</text><text x="64" y="${y+43}" font-size="8.5" fill="#58689a">${s[2]}</text>${i<3?arw(30,y+54,y+73):""}`}).join("")}</svg>`};
const ui=()=>{const card=i=>{const y=68+i*62;return `<rect x="10" y="${y}" width="180" height="54" rx="8" fill="#fff" stroke="#c5cde0"/><rect x="16" y="${y+6}" width="58" height="42" rx="5" fill="url(#g)"/><rect x="82" y="${y+10}" width="70" height="6" rx="3" fill="#141b2d" opacity=".8"/><rect x="82" y="${y+22}" width="50" height="5" rx="2.5" fill="#9fb0d6"/><rect x="82" y="${y+34}" width="28" height="9" rx="4.5" fill="#dbe5fb"/><rect x="114" y="${y+34}" width="28" height="9" rx="4.5" fill="#dbe5fb"/><rect x="156" y="${y+8}" width="28" height="12" rx="6" fill="#2457c5"/>`};return `<svg viewBox="0 0 200 260" xmlns="http://www.w3.org/2000/svg" font-family="Space Grotesk,sans-serif"><defs><linearGradient id="g" x1="0" y1="0" x2="1" y2="1"><stop offset="0" stop-color="#7fa6f0"/><stop offset="1" stop-color="#22d3ee"/></linearGradient></defs><rect width="200" height="260" fill="#f4f7ff"/><rect x="10" y="10" width="180" height="20" rx="10" fill="#fff" stroke="#c5cde0"/><text x="22" y="24" font-size="8" fill="#7a869f">Search area, college, office…</text>${["Area","Budget","Sharing","Food"].map((t,i)=>`<rect x="${10+i*46}" y="38" width="40" height="16" rx="8" fill="#dbe5fb"/><text x="${30+i*46}" y="49" text-anchor="middle" font-size="7.5" fill="#1e3f8f">${t}</text>`).join("")}${card(0)+card(1)+card(2)}</svg>`};
const arch=()=>`<svg viewBox="0 0 220 280" xmlns="http://www.w3.org/2000/svg" font-family="Space Grotesk,sans-serif">${MK}<rect width="220" height="280" fill="#f4f7ff"/>${bx(30,8,160,46,"Browser","HTML · CSS · JavaScript")}${arw(110,54,76)}${bx(30,78,160,46,"PHP back end","handles requests")}${arw(110,124,146)}<rect x="30" y="148" width="160" height="124" rx="10" fill="#fff" stroke="#0e9f6e"/><text x="110" y="166" text-anchor="middle" font-size="11" font-weight="700" fill="#0e9f6e">MySQL</text><rect x="44" y="176" width="132" height="86" rx="4" fill="#f4f7ff" stroke="#c5cde0"/><rect x="44" y="176" width="132" height="16" rx="4" fill="#dff3e8"/><text x="52" y="187" font-size="8" font-family="monospace" fill="#141b2d">listings (illustrative)</text>${["id","name","area","rent"].map((c,i)=>`<text x="52" y="${204+i*14}" font-size="8" font-family="monospace" fill="#58689a">${c}</text><line x1="48" x2="172" y1="${208+i*14}" y2="${208+i*14}" stroke="#e2e8f5"/>`).join("")}</svg>`;
const fscan=()=>`<svg class="bg" viewBox="0 0 160 200" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="fg" x1="0" y1="0" x2="0" y2="1"><stop offset="0" stop-color="#06122b"/><stop offset="1" stop-color="#0a3a5c"/></linearGradient></defs><rect width="160" height="200" fill="url(#fg)"/>${Array.from({length:9},(_,i)=>`<path d="M0 ${i*24}H160M${i*20} 0V200" stroke="#22d3ee" stroke-opacity=".08"/>`).join("")}<ellipse cx="80" cy="82" rx="30" ry="40" fill="none" stroke="#22d3ee" stroke-width="1.2"/>${[[68,72],[92,72],[80,86],[70,100],[90,100],[80,104]].map(p=>`<circle cx="${p[0]}" cy="${p[1]}" r="1.6" fill="#22d3ee"/>`).join("")}<path d="M38 34v-10h10M122 34v-10h-10M38 130v10h10M122 130v10h-10" stroke="#3b82f6" stroke-width="2" fill="none"/><line x1="38" x2="122" y1="40" y2="40" stroke="#22d3ee" stroke-width=".8"><animate attributeName="y1" values="40;128;40" dur="4s" repeatCount="indefinite"/><animate attributeName="y2" values="40;128;40" dur="4s" repeatCount="indefinite"/></line></svg>`;
const sky=()=>`<svg class="bg" viewBox="0 0 160 200" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="sg" x1="0" y1="0" x2="0" y2="1"><stop offset="0" stop-color="#0b2250"/><stop offset="1" stop-color="#0a4a5c"/></linearGradient></defs><rect width="160" height="200" fill="url(#sg)"/>${[[10,90,28],[42,60,34],[80,100,26],[110,50,36]].map(([x,y,w])=>`<rect x="${x}" y="${y+20}" width="${w}" height="${180-y}" fill="#0b1a36" stroke="#2b4a8a" stroke-width=".5"/>${Array.from({length:Math.floor((160-y)/14)},(_,r)=>[0,1,2].map(c=>`<rect x="${x+4+c*(w/3.2)}" y="${y+28+r*14}" width="5" height="6" fill="${(r+c+x)%3?"#fde68a":"#1e3a6e"}" opacity=".85"/>`).join("")).join("")}`).join("")}</svg>`;
const fut=()=>`<svg viewBox="0 0 160 120" xmlns="http://www.w3.org/2000/svg" style="width:80%;margin:auto" role="img" aria-label="Illustration: a path of finished and future projects"><path d="M10 100C40 95 50 70 70 66S100 50 118 40" fill="none" stroke="#22d3ee" stroke-width="1.5"/><path d="M118 40C130 34 140 24 152 14" fill="none" stroke="#3b82f6" stroke-dasharray="3 3"/>${[[10,100],[40,92],[70,66],[96,56],[118,40]].map(p=>`<circle cx="${p[0]}" cy="${p[1]}" r="4" fill="#22d3ee"/>`).join("")}${[[134,28],[152,14]].map(p=>`<circle cx="${p[0]}" cy="${p[1]}" r="4" fill="none" stroke="#3b82f6" stroke-dasharray="2 2"/>`).join("")}</svg>`;
const ov='<div class="ov"></div>',cv=(k,t,p)=>`${ov}<div class="tx"><div class="eyebrow">${k}</div><h3>${t}</h3><p>${p}</p></div>`;
const th1=aer(3,0),th2='<svg viewBox="0 0 40 40"><rect width="40" height="40" fill="#0a3a5c"/><ellipse cx="20" cy="19" rx="8" ry="10" fill="none" stroke="#22d3ee"/></svg>',th3='<svg viewBox="0 0 40 40"><rect width="40" height="40" fill="#0b2250"/><rect x="6" y="14" width="10" height="26" fill="#2b4a8a"/><rect x="20" y="8" width="12" height="32" fill="#3b82f6"/></svg>';
const F=[
["cov dk",bg(aer(11,1))+cv("Portfolio · 2026","Selected Work","Three chapters · drag, swipe or tap Next →")],
["",`<div class="pad"><div class="eyebrow">Contents</div><h3>Three chapters</h3><div class="toc"><button data-j="1"><span class="th">${th1}</span><span><b>01</b> Land Cover Segmentation</span></button><button data-j="4"><span class="th">${th2}</span><span><b>02</b> Facial Recognition Attendance</span></button><button data-j="6"><span class="th">${th3}</span><span><b>03</b> PG Finder</span></button></div><p>Tap any figure to enlarge. <span class="tg">ILLUSTRATIVE</span> is concept art; <span class="tg w">PLACEHOLDER</span> awaits a real screenshot.</p></div>`],
["cov",bg(aer(3,0))+cv("Chapter 01","Geospatial Land Cover Segmentation","Teaching a network to read the ground from above, one pixel at a time.")],
["",`<div class="pad"><div class="num">01</div><div class="eyebrow">The problem</div><h3>Reading the ground from the air</h3><p>Land-use maps are slow to draw by hand. Aerial scenes blend water, vegetation, fields and buildings with soft, irregular borders.</p>${fig(aer(5,0),"One scene can hold several land-cover classes at once.")}<div class="stats"><div><b>Mixed</b><small>classes per scene</small></div><div><b>Fuzzy</b><small>natural edges</small></div><div><b>Varied</b><small>object scale</small></div></div></div>`],
["",`<div class="pad"><div class="num">02</div><div class="eyebrow">Dataset</div><h3>Imagery in, masks out</h3><div class="two">${fig(aer(7,0),"Aerial tile")}${fig(aer(7,1),"Class mask")}</div>${bd(CL.map(c=>[c[0],c[1]]))}<p>Sample classes shown for illustration — <i>[add your dataset name &amp; real class list]</i>.</p></div>`],
["",`<div class="pad"><div class="num">03</div><div class="eyebrow">Model</div><h3>Architecture</h3><div class="two">${fig(pipe(),"DeepLabV3+ with a ResNet-50 backbone")}<div><h4>Encoder</h4><p>ResNet-50 extracts features from the image.</p><h4>ASPP</h4><p>Atrous convolutions read context at several scales.</p><h4>Decoder</h4><p>Recovers sharp object boundaries for the final per-pixel mask.</p></div></div></div>`],
["",`<div class="pad"><div class="num">04</div><div class="eyebrow">Results</div><h3>Input vs prediction</h3><div class="two">${fig(aer(9,0),"Input")}${fig(aer(9,1),"Prediction")}</div><div class="stats"><div><b>—</b><small>mIoU</small></div><div><b>—</b><small>pixel accuracy</small></div><div><b>—</b><small>F1</small></div></div><p>Left blank on purpose — <i>[add your real metrics]</i>. Research paper in submission.</p></div>`],
["",`<div class="pad"><div class="num">05</div><div class="eyebrow">Stack &amp; learnings</div><h3>What it took</h3>${bd([["Python","#3776ab"],["PyTorch","#ee4c2c"],["DeepLabV3+","#2457c5"],["ResNet-50","#0e9f6e"],["Aerial imagery","#8c8a47"]])}<h4>Key learnings</h4><ul><li>Context modules matter for multi-scale scenes.</li><li>Boundaries are the hard part — the decoder earns its keep.</li><li>Class imbalance shapes what the model learns.</li></ul></div>`],
["cov dk",fscan()+cv("Chapter 02","Facial Recognition Attendance","Cameras take the roll call so class time doesn’t have to.")],
["",`<div class="pad"><div class="num">01</div><div class="eyebrow">Problem &amp; workflow</div><h3>From camera to attendance sheet</h3><div class="two">${fig(flow(),"End-to-end workflow")}<div><h4>Problem</h4><p>Manual roll-calls cost time and invite errors.</p><h4>Objective</h4><p>Recognise faces from a camera feed and record attendance automatically, even in real-world conditions.</p></div></div></div>`],
["",`<div class="pad"><div class="num">02</div><div class="eyebrow">Approach</div><h3>Detect, recognise, record</h3><div class="stats"><div><b>90%+</b><small>real-world accuracy</small></div><div><b>Custom</b><small>trained detection</small></div><div><b>Flask</b><small>web interface</small></div></div><p>Face detection custom-trained with OpenCV, wrapped in a Flask app for everyday use.</p>${bd([["OpenCV","#0e9f6e"],["Python","#3776ab"],["Flask","#141b2d"]])}</div>`],
["",`<div class="pad"><div class="num">03</div><div class="eyebrow">Interface &amp; learnings</div>${ph("Attendance app screenshot")}<h4>Key learnings</h4><p>Real-world accuracy depends on lighting, angle and data variety — a clean demo isn’t the finish line.</p></div>`],
["cov dk",sky()+cv("Chapter 03","PG Finder","Finding a place to stay, compared side by side.")],
["",`<div class="pad"><div class="num">01</div><div class="eyebrow">Search &amp; filter</div><h3>Find, filter, compare</h3><div class="two">${fig(ui(),"Concept sketch of search &amp; filters — not the real UI")}<div><h4>Problem</h4><p>Finding a suitable PG means hopping between listings with no easy comparison.</p><h4>Features</h4><p>Accommodation discovery and comparison. <i>[list your real features]</i></p></div></div></div>`],
["",`<div class="pad"><div class="num">02</div><div class="eyebrow">Implementation</div><h3>Architecture</h3><div class="two">${fig(arch(),"Front end → PHP → MySQL (schema illustrative)")}<div><h4>Front end</h4><p>HTML, CSS and JavaScript interface.</p><h4>Back end</h4><p>PHP handles requests and logic.</p><h4>Database</h4><p>MySQL stores the listings.</p></div></div>${bd([["PHP","#777bb3"],["MySQL","#00758f"],["HTML","#e34f26"],["CSS","#1572b6"],["JavaScript","#d4b800"]])}</div>`],
["",`<div class="pad"><div class="num">03</div><div class="eyebrow">Listings &amp; learnings</div>${ph("PG Finder listing screenshot")}<h4>Key learnings</h4><ul><li>Designing a relational schema for listings.</li><li>Wiring the front end to the back end.</li><li>Building filters around how people choose a place.</li></ul></div>`],
["dk",`<div class="pad" style="justify-content:center;text-align:center"><div class="eyebrow">Epilogue</div><h3 style="font-weight:300;font-size:2.1em">The journey is still being written.</h3>${fut()}<p>More projects, more experiments and more chapters ahead.</p></div>`],
["cov dk",bg(aer(2,1))+cv("Sahana Shetty","Thank you for reading","")]];
const N=F.length/2,bk=$("#book"),lb=$("#lb");let cur=0,mv=false;const leaves=[];
const face=k=>`<div class="face ${F[k][0]}${k%2?" b":""}">${F[k][1]}${k>1&&k<17?`<span class="pn ${k%2?"l":"r"}">${String(k).padStart(2,"0")}</span>`:""}</div>`;
for(let i=0;i<N;i++){const l=document.createElement("div");l.className="leaf";l.innerHTML=face(2*i)+face(2*i+1);bk.append(l);leaves.push(l)}
const CH=f=>f<2?"Cover & contents":f<8?"Ch. 01 · Land Cover":f<12?"Ch. 02 · Attendance":f<16?"Ch. 03 · PG Finder":"Epilogue";
function up(init){leaves.forEach((l,i)=>{const f=i<cur;l.classList.toggle("f",f);clearTimeout(l.t);const z=f?i:N-i;if(init)l.style.zIndex=z;else{l.style.zIndex=100;l.t=setTimeout(()=>l.style.zIndex=z,550)}});
bk.style.transform=`rotateX(8deg) translateX(${cur==0?-bk.offsetWidth/2:cur==N?bk.offsetWidth/2:0}px)`;$("#prev").disabled=cur==0;$("#next").disabled=cur==N;$("#pb").style.width=cur/N*100+"%";$("#pg").textContent=`${CH(Math.min(2*cur,17))} · ${cur==0?"closed":cur==N?"end":`pages ${2*cur-1}–${2*cur}`}`}
const go=d=>{cur=Math.max(0,Math.min(N,cur+d));up()};
$("#prev").onclick=()=>go(-1);$("#next").onclick=()=>go(1);$("#toc").onclick=()=>{cur=1;up()};
bk.querySelectorAll("[data-j]").forEach(b=>b.onclick=()=>{cur=+b.dataset.j;up()});
const open=f=>{$("#lbc").innerHTML=f.querySelector("svg").outerHTML+`<p>${f.querySelector("figcaption").textContent}</p>`;lb.hidden=false;$("#lbx").focus()};
bk.addEventListener("click",e=>{const f=e.target.closest(".z");if(f&&!mv)open(f)});
bk.addEventListener("keydown",e=>{if(e.key=="Enter"&&e.target.classList.contains("z"))open(e.target)});
lb.onclick=e=>{if(e.target==lb||e.target.id=="lbx")lb.hidden=true};
addEventListener("keydown",e=>{if(e.key=="Escape")lb.hidden=true;if(!lb.hidden)return;if(e.key=="ArrowRight")go(1);if(e.key=="ArrowLeft")go(-1)});
addEventListener("resize",()=>up(true));
let sx=null;$("#stage").addEventListener("pointerdown",e=>{if(e.target.closest("button"))return;sx=e.clientX});
addEventListener("pointerup",e=>{if(sx===null)return;const d=e.clientX-sx;sx=null;mv=Math.abs(d)>6;if(d<-45)go(1);else if(d>45)go(-1)});
up(true)})();
// gallery
(()=>{const E=[["ACADEMIC","B.Tech, Information Technology","CMR University, Bengaluru · 2026 · CGPA 9.16/10"],["ACADEMIC","Chancellor’s List","CMR University"],["CERTIFICATION","Software Testing","NPTEL"],["CERTIFICATION","Full-Stack Web Development","Internshala"],["HACKATHON","Google Girl Hackathon 2025","Solo participant — designed and pitched an AI solution to a panel of technical judges."],["HACKATHON","NHAI Road Safety Hackathon 2024","Team lead — data-backed road safety policy brief; 300+ competing teams."],["HACKATHON","VoxaFit · Innovatex 3.0, 2024","Team lead — built and demoed a fitness analytics app at Presidency College."],["INTERNSHIP","[ Add your internship ]","Company, role and what you shipped."]];
const g=$("#gal");E.forEach((e,i)=>{const d=document.createElement("div");d.className="ex rv"+(i==7?" ph2":"");d.style.transitionDelay=i%4*.08+"s";d.innerHTML=`<small>${e[0]}</small><h3>${e[1]}</h3><p>${e[2]}</p>`;
if(!reduce){d.onpointermove=ev=>{const r=d.getBoundingClientRect(),x=(ev.clientX-r.left)/r.width-.5,y=(ev.clientY-r.top)/r.height-.5;d.style.transform=`rotateY(${x*12}deg) rotateX(${-y*12}deg) translateZ(10px)`;d.style.transitionDelay="0s"};d.onpointerleave=()=>d.style.transform=""}
g.append(d);io.observe(d)})})();
// terminal
(()=>{const tm=$("#tm"),L=[`<span class="p-mu">$</span> whoami`,`sahana-shetty · software engineer · ai/ml`,`<span class="p-mu">$</span> ls ./connect`,`<a href="${LINKS.github}" target="_blank" rel="noopener">github</a>   <a href="${LINKS.linkedin}" target="_blank" rel="noopener">linkedin</a>   <a href="${LINKS.email}">email</a>`,`<span class="p-mu">$</span> <span class="cur"></span>`];
let started=false;new IntersectionObserver((e,o)=>{if(!e[0].isIntersecting||started)return;started=true;let i=0;const s=()=>{if(i>=L.length)return;tm.innerHTML=L.slice(0,++i).join("\n");setTimeout(s,reduce?0:650)};s()},{threshold:.4}).observe(tm)})();
</script></body></html>
