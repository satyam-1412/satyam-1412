<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Satyam Sangle · Full Stack Developer</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;500;700;800&family=IBM+Plex+Sans:wght@400;500&display=swap" rel="stylesheet">
<style>
:root{--bg:#0a0e14;--surface:#0f1620;--ink:#d3deec;--muted:#7f90a8;--accent:#39ff9c;--accent-ink:#04110a;--accent2:#5ccfff;--line:#1d2a3b;--mint:#39ff9c}
:root[data-accent="cyan"]{--accent:#5ccfff;--accent-ink:#04121a;--accent2:#c792ff;--mint:#5ccfff}
:root[data-accent="amber"]{--accent:#ffb454;--accent-ink:#1a1004;--accent2:#ff6b8a;--mint:#ffb454}
*{box-sizing:border-box}html{scroll-behavior:smooth}
body{margin:0;color:var(--ink);font:400 15.5px/1.65 "IBM Plex Sans",system-ui,sans-serif;background:var(--bg);
 background-image:linear-gradient(var(--line) 1px,transparent 1px),linear-gradient(90deg,var(--line) 1px,transparent 1px);background-size:44px 44px;background-attachment:fixed}
body::before{content:"";position:fixed;inset:0;background:radial-gradient(ellipse at 20% 0%,transparent 0,var(--bg) 75%);pointer-events:none;z-index:0}
.wrap,footer{position:relative;z-index:1}
a{color:inherit}:focus-visible{outline:2px solid var(--accent);outline-offset:3px}
.mono,h1,h2,h3,.role,.tag,.chip,.theme,.num,.live,.meta,small,.links a,.cta a,.crumb{font-family:"JetBrains Mono",ui-monospace,monospace}
.wrap{max-width:1140px;margin:0 auto;padding:40px 24px;display:grid;grid-template-columns:330px 1fr;gap:40px}
@media(max-width:880px){.wrap{grid-template-columns:1fr;gap:28px;padding:22px 16px}}
.win{background:color-mix(in srgb,var(--surface) 92%,transparent);border:1px solid var(--line);border-radius:12px;overflow:hidden;box-shadow:0 0 0 1px #0006,0 20px 50px -25px var(--accent)}
.bar-top{display:flex;align-items:center;gap:7px;padding:10px 14px;border-bottom:1px solid var(--line);background:#0b121b;font:12px "JetBrains Mono",monospace;color:var(--muted)}
.bar-top i{width:10px;height:10px;border-radius:50%;background:#ff5f57}.bar-top i:nth-child(2){background:#febc2e}.bar-top i:nth-child(3){background:#28c840}
.bar-top span{margin-left:8px}
.body{padding:20px}
aside{position:sticky;top:28px;align-self:start}@media(max-width:880px){aside{position:static}}
.avatar{width:96px;height:96px;border-radius:14px;background:var(--line);object-fit:cover;display:block;border:2px solid var(--accent);box-shadow:0 0 22px -4px var(--accent)}
.prompt{font:13px "JetBrains Mono",monospace;color:var(--muted);margin:18px 0 4px}.prompt b{color:var(--accent);font-weight:500}
h1{font:800 1.9rem/1.1 "JetBrains Mono",monospace;margin:0 0 8px;letter-spacing:-.03em}
.role{font-size:.95rem;color:var(--accent);min-height:1.7em;margin:0 0 10px}
.role::after{content:"";display:inline-block;width:.6em;height:1.05em;background:var(--accent);margin-left:4px;vertical-align:-3px;animation:blink 1s steps(1) infinite}
@keyframes blink{50%{opacity:0}}
.bio{margin:0 0 18px;color:var(--muted);font-size:.93rem}
.links{display:grid;gap:8px;margin:0;padding:0;list-style:none}
.links a{display:flex;align-items:center;gap:10px;padding:9px 12px;border-radius:8px;background:#0b121b;border:1px solid var(--line);text-decoration:none;font-size:.85rem;transition:all .15s}
.links a::before{content:">";color:var(--accent)}
.links a:hover{border-color:var(--accent);color:var(--accent);box-shadow:0 0 16px -6px var(--accent);transform:translateX(3px)}
.links .ico{display:none}
.theme{margin-top:16px;background:none;border:1px solid var(--line);color:var(--muted);padding:7px 12px;border-radius:8px;cursor:pointer;font-size:.78rem}
.theme:hover{color:var(--accent);border-color:var(--accent)}
main section{margin-bottom:32px}
h2{font:700 1.15rem/1.2 "JetBrains Mono",monospace;margin:0;color:var(--ink)}
h2 .p{color:var(--accent);margin-right:8px}
.sub{color:var(--muted);margin:0 0 16px;font-size:.88rem}
.chips,.tabs{display:flex;flex-wrap:wrap;gap:8px}
.tag{padding:5px 11px;border-radius:6px;border:1px solid var(--line);background:#0b121b;font-size:.8rem;color:var(--accent2)}
.chip{padding:6px 12px;border-radius:6px;border:1px solid var(--line);background:transparent;color:var(--muted);font-size:.8rem;cursor:pointer}
.chip:hover{color:var(--ink)}
.chip[aria-pressed="true"]{background:var(--accent);color:var(--accent-ink);border-color:var(--accent)}
.cards{display:grid;grid-template-columns:repeat(auto-fill,minmax(210px,1fr));gap:12px}
.card{padding:16px;border-radius:10px;background:#0b121b;border:1px solid var(--line);text-decoration:none;display:block;transition:all .15s}
a.card:hover{border-color:var(--accent);box-shadow:0 0 22px -8px var(--accent);transform:translateY(-2px)}
.card small{color:var(--muted);display:block;font-size:.76rem}
.num{font-weight:800;font-size:2.3rem;line-height:1.1;margin:6px 0 2px;color:var(--accent);text-shadow:0 0 18px color-mix(in srgb,var(--accent) 55%,transparent)}
.live{display:inline-block;font-size:.66rem;padding:1px 7px;border-radius:4px;border:1px solid var(--accent);color:var(--accent);margin-left:8px;vertical-align:2px;animation:pulse 2s ease-in-out infinite}
@keyframes pulse{50%{opacity:.45}}
.bar{height:5px;border-radius:99px;background:var(--line);overflow:hidden;margin-top:12px}
.bar i{display:block;height:100%;width:0;background:linear-gradient(90deg,var(--accent2),var(--accent));transition:width 1.2s ease}
.ach{margin:0;padding:0;list-style:none;display:grid;gap:8px;font-size:.92rem}
.ach li::before{content:"✔ ";color:var(--accent)}
.graph img{width:100%;display:block;filter:invert(1) hue-rotate(180deg) saturate(1.2);border-radius:6px}
.tools{display:flex;flex-wrap:wrap;gap:10px;margin-bottom:16px}
.tools input{flex:1 1 200px;padding:10px 14px;border-radius:8px;border:1px solid var(--line);background:#0b121b;color:var(--ink);font:13px "JetBrains Mono",monospace}
.tools input::placeholder{color:var(--muted)}
.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(250px,1fr));gap:12px}
.repo{display:flex;flex-direction:column;gap:8px}
.repo h3{margin:0;font-size:.98rem;color:var(--accent2);word-break:break-word}
.repo p{margin:0;color:var(--muted);font-size:.86rem;flex:1}
.meta{display:flex;flex-wrap:wrap;gap:12px;font-size:.74rem;color:var(--muted)}
.dot{display:inline-block;width:9px;height:9px;border-radius:50%;margin-right:6px}
.state{padding:20px;border:1px dashed var(--line);border-radius:10px;color:var(--muted);font:13px "JetBrains Mono",monospace}
.skeleton{height:130px;border-radius:10px;background:linear-gradient(90deg,#0b121b,var(--line),#0b121b);background-size:200% 100%;animation:sh 1.4s linear infinite}
@keyframes sh{to{background-position:-200% 0}}
.cta{text-align:left}
.cta p{margin:6px 0 16px;color:var(--muted)}
.cta a{display:inline-block;padding:10px 16px;border-radius:8px;background:var(--accent);color:var(--accent-ink);font-weight:700;font-size:.85rem;text-decoration:none;margin:0 8px 8px 0}
.cta a:nth-of-type(2){background:transparent;color:var(--accent);border:1px solid var(--accent)}
footer{grid-column:1/-1;color:var(--muted);font:12px "JetBrains Mono",monospace;border-top:1px solid var(--line);padding-top:16px}
@media(prefers-reduced-motion:reduce){*{animation:none!important;transition:none!important}html{scroll-behavior:auto}}
</style>
</head>
<body>
<div class="wrap">
<aside class="win">
  <div class="bar-top"><i></i><i></i><i></i><span>~/satyam</span></div>
  <div class="body">
  <img class="avatar" id="avatar" alt="Satyam Sangle" width="96" height="96">
  <p class="prompt"><b>$</b> whoami</p>
  <h1>Satyam Sangle</h1>
  <p class="role" id="role" aria-label="Full Stack Developer and Competitive Programmer"></p>
  <p class="bio">B.Tech ECE student at IIIT Jabalpur. I build web apps and solve algorithm problems.</p>
  <p class="prompt"><b>$</b> ls links/</p>
  <ul class="links" id="links"></ul>
  <button class="theme" id="theme" type="button">theme: green</button>
  </div>
</aside>
<main>
<section id="about" class="win "><div class="bar-top"><i></i><i></i><i></i><span>about.md</span></div><div class="body"><h2><span class="p">$</span>cat about.md</h2><p>I'm a student at <b>IIIT Jabalpur</b> pursuing B.Tech in Electronics &amp; Communication Engineering. I like building scalable web applications and solving hard algorithmic problems. Right now I'm focused on full stack development with Python and Flask, competitive programming, and building production-ready apps.</p><div class="chips" id="skills"></div></div></section>
<section id="coding" class="win "><div class="bar-top"><i></i><i></i><i></i><span>stats.sh</span></div><div class="body"><h2><span class="p">$</span>./stats.sh <span class="live" id="liveBadge" hidden>live</span></h2><p class="sub">Values marked live are fetched from the platforms when this page opens.</p><div class="cards" id="cp"></div></div></section>
<section id="achievements" class="win "><div class="bar-top"><i></i><i></i><i></i><span>achievements.log</span></div><div class="body"><h2><span class="p">$</span>tail achievements.log</h2><br><ul class="ach" id="ach"></ul></div></section>
<section id="activity" class="win "><div class="bar-top"><i></i><i></i><i></i><span>git-log</span></div><div class="body"><h2><span class="p">$</span>git log --graph</h2><br><div class="graph"><img id="graph" alt="GitHub contribution graph" loading="lazy"></div></div></section>
<section id="projects" class="win "><div class="bar-top"><i></i><i></i><i></i><span>projects/</span></div><div class="body"><h2><span class="p">$</span>ls projects/</h2><p class="sub" id="sub">fetching from GitHub…</p><div class="tools"><input id="q" type="search" placeholder="grep projects..." aria-label="Search projects"><div class="chips" id="chips" role="group" aria-label="Filter by language"></div></div><div class="grid" id="grid" aria-live="polite"><div class="skeleton"></div><div class="skeleton"></div><div class="skeleton"></div></div></div></section>
<section id="contact" class="win cta"><div class="bar-top"><i></i><i></i><i></i><span>contact.sh</span></div><div class="body"><h2><span class="p">$</span>./contact.sh</h2><p>Open to opportunities, collaborations and interesting projects.</p><a href="mailto:sanglesatyam@gmail.com">Email me</a><a href="https://www.linkedin.com/in/satyam-sangle-20a096324/" target="_blank" rel="noopener">Connect on LinkedIn</a></div></section>
</main>
<footer>// projects, ratings and activity update automatically from GitHub, Codeforces and LeetCode</footer>
</div>

<script>
/* ============ EDIT THIS PART ============ */
const CONFIG = {
  github: "satyam-1412",
  leetcode: "satyam_1412",
  codeforces: "sanglesatyam",
  hideForks: true,
  pinned: [],
  roles: ["Full Stack Developer", "Competitive Programmer", "Python & Flask builder", "IIIT Jabalpur ECE student"],
  links: [
    {label:"GitHub", icon:"🐙", url:"https://github.com/satyam-1412"},
    {label:"LinkedIn", icon:"💼", url:"https://www.linkedin.com/in/satyam-sangle-20a096324/"},
    {label:"LeetCode", icon:"🧩", url:"https://leetcode.com/u/satyam_1412"},
    {label:"Codeforces", icon:"📈", url:"https://codeforces.com/profile/sanglesatyam"},
    {label:"Email", icon:"✉️", url:"mailto:sanglesatyam@gmail.com"}
  ],
  skills: ["Python","C","C++","JavaScript","HTML/CSS","Flask","Git","GitHub","VS Code","Jupyter","Data Structures & Algorithms","Database Design","API Development"],
  /* shown if a live fetch fails */
  fallback: {leetcodeSolved: 375, cfRating: 1258, cfMax: 1258, cfRank: "pupil"},
  codechef: {handle:"satyam_2004", stars: 2},
  achievements: [
    "Participated in “Can U Hack It”, a 24-hour intra-college hackathon",
    "98.58 percentile in JEE Mains and qualified JEE Advanced"
  ]
};
/* ======================================== */

const $=id=>document.getElementById(id);
const esc=s=>String(s??"").replace(/[&<>"']/g,c=>({"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;","'":"&#39;"}[c]));
const LC={JavaScript:"#f1e05a",TypeScript:"#3178c6",Python:"#3572a5",HTML:"#e34c26",CSS:"#8b6fe8",Java:"#b07219",C:"#888","C++":"#f34b7d",Jupyter:"#da5b0b","Jupyter Notebook":"#da5b0b"};
const timeout=(ms)=>{const c=new AbortController();setTimeout(()=>c.abort(),ms);return c.signal};

/* typing roles */
(function(){
  const el=$("role"),r=CONFIG.roles;let i=0,j=0,del=false;
  if(matchMedia("(prefers-reduced-motion:reduce)").matches){el.textContent=r[0];return}
  (function tick(){
    const w=r[i];el.textContent=w.slice(0,j);
    if(!del&&j===w.length){del=true;return setTimeout(tick,1600)}
    if(del&&j===0){del=false;i=(i+1)%r.length}
    j+=del?-1:1;setTimeout(tick,del?35:70);
  })();
})();

/* links, skills, achievements */
$("links").innerHTML=CONFIG.links.map(l=>`<li><a href="${esc(l.url)}"${/^https?:/.test(l.url)?' target="_blank" rel="noopener"':""}><span class="ico" aria-hidden="true">${l.icon}</span>${esc(l.label)}</a></li>`).join("");
$("skills").innerHTML=CONFIG.skills.map(s=>`<span class="tag">${esc(s)}</span>`).join("");
$("ach").innerHTML=CONFIG.achievements.map(a=>`<li>${esc(a)}</li>`).join("");

/* avatar with fallback */
const av=$("avatar");
av.onerror=()=>{av.style.display="none"};
av.src=`https://github.com/${CONFIG.github}.png?size=200`;
fetch(`https://api.github.com/users/${CONFIG.github}`).then(r=>r.ok?r.json():null).then(p=>{if(p&&p.avatar_url){av.style.display="";av.src=p.avatar_url}}).catch(()=>{});

/* accent theme */
const root=document.documentElement,accents=["green","cyan","amber"],hex={green:"39ff9c",cyan:"5ccfff",amber:"ffb454"};
function setAccent(a){
  if(a==="green")delete root.dataset.accent;else root.dataset.accent=a;
  $("theme").textContent="theme: "+a;
  $("graph").src=`https://ghchart.rshah.org/${hex[a]}/${CONFIG.github}`;
  try{localStorage.setItem("accent",a)}catch{}
}
let cur="green";try{cur=localStorage.getItem("accent")||"green"}catch{}
if(!accents.includes(cur))cur="green";
setAccent(cur);
$("theme").onclick=()=>{cur=accents[(accents.indexOf(cur)+1)%accents.length];setAccent(cur)};

/* count-up */
function countUp(el,to){
  if(matchMedia("(prefers-reduced-motion:reduce)").matches){el.textContent=to;return}
  const t0=performance.now();
  (function f(t){const p=Math.min((t-t0)/1000,1);el.textContent=Math.round(to*(1-Math.pow(1-p,3)));if(p<1)requestAnimationFrame(f)})(t0);
}

/* coding stats */
const cap=s=>s?s[0].toUpperCase()+s.slice(1):"";
function cpCard({name,url,value,label,sub,live,bar}){
  return `<a class="card" href="${esc(url)}" target="_blank" rel="noopener"><small>${esc(name)}${live?'<span class="live">live</span>':""}</small><div class="num" data-to="${value}">0</div><small>${esc(label)}</small>${sub?`<small>${esc(sub)}</small>`:""}${bar!=null?`<div class="bar"><i data-w="${bar}"></i></div>`:""}</a>`;
}
async function loadStats(){
  const F=CONFIG.fallback;let lc={solved:F.leetcodeSolved,live:false},cf={rating:F.cfRating,max:F.cfMax,rank:F.cfRank,live:false};
  const [a,b]=await Promise.allSettled([
    fetch(`https://leetcode-stats-api.herokuapp.com/${CONFIG.leetcode}`,{signal:timeout(6000)}).then(r=>r.json()),
    fetch(`https://codeforces.com/api/user.info?handles=${CONFIG.codeforces}`,{signal:timeout(6000)}).then(r=>r.json())
  ]);
  if(a.status==="fulfilled"&&a.value.status==="success")lc={solved:a.value.totalSolved,easy:a.value.easySolved,med:a.value.mediumSolved,hard:a.value.hardSolved,live:true};
  if(b.status==="fulfilled"&&b.value.status==="OK"){const u=b.value.result[0];cf={rating:u.rating??0,max:u.maxRating??0,rank:u.rank,maxRank:u.maxRank,live:true}}
  const cards=[
    {name:"LeetCode",url:`https://leetcode.com/u/${CONFIG.leetcode}`,value:lc.solved,label:"problems solved",sub:lc.live?`${lc.easy} easy · ${lc.med} medium · ${lc.hard} hard`:"",live:lc.live,bar:Math.min(lc.solved/500*100,100)},
    {name:"Codeforces",url:`https://codeforces.com/profile/${CONFIG.codeforces}`,value:cf.rating,label:`current rating${cf.rank?", "+cap(cf.rank):""}`,sub:cf.max?`Peak ${cf.max}${cf.maxRank?" ("+cap(cf.maxRank)+")":""}`:"",live:cf.live,bar:Math.min(cf.rating/2400*100,100)},
    {name:"CodeChef",url:`https://www.codechef.com/users/${CONFIG.codechef.handle}`,value:CONFIG.codechef.stars,label:"star rating",sub:"@"+CONFIG.codechef.handle,live:false}
  ];
  $("cp").innerHTML=cards.map(cpCard).join("");
  $("liveBadge").hidden=!(lc.live||cf.live);
  document.querySelectorAll(".num").forEach(n=>countUp(n,+n.dataset.to));
  requestAnimationFrame(()=>document.querySelectorAll(".bar i").forEach(i=>i.style.width=i.dataset.w+"%"));
}

/* repos */
let repos=[],activeLang="All";
async function loadRepos(){
  try{
    const r=await fetch(`https://api.github.com/users/${CONFIG.github}/repos?per_page=100&sort=updated`);
    if(!r.ok)throw new Error(r.status===403?"GitHub rate limit reached. Try again in a few minutes.":"Could not load repositories. Check the GitHub username in CONFIG.");
    repos=await r.json();
    if(CONFIG.hideForks)repos=repos.filter(x=>!x.fork);
    repos.sort((a,b)=>{const pa=CONFIG.pinned.indexOf(a.name),pb=CONFIG.pinned.indexOf(b.name);
      if(pa!==-1||pb!==-1)return(pa===-1?99:pa)-(pb===-1?99:pb);return new Date(b.pushed_at)-new Date(a.pushed_at)});
    const langs=[...new Set(repos.map(x=>x.language).filter(Boolean))];
    $("chips").innerHTML=["All",...langs].map(l=>`<button type="button" class="chip" data-lang="${esc(l)}" aria-pressed="${l==="All"}">${esc(l)}</button>`).join("");
    $("sub").textContent=`${repos.length} projects, most recently active first.`;
    renderRepos();
  }catch(e){$("sub").textContent="";$("grid").innerHTML=`<div class="state">${esc(e.message)}</div>`}
}
function renderRepos(){
  const q=$("q").value.trim().toLowerCase();
  const l=repos.filter(r=>(activeLang==="All"||r.language===activeLang)&&(!q||(r.name+" "+(r.description||"")+" "+(r.topics||[]).join(" ")).toLowerCase().includes(q)));
  $("grid").innerHTML=l.length?l.map(r=>`<a class="card repo" href="${esc(r.homepage&&/^https?:/.test(r.homepage)?r.homepage:r.html_url)}" target="_blank" rel="noopener"><h3>${esc(r.name)}</h3><p>${esc(r.description||"No description yet.")}</p><div class="meta">${r.language?`<span><i class="dot" style="background:${LC[r.language]||"var(--accent)"}"></i>${esc(r.language)}</span>`:""}<span>★ ${r.stargazers_count}</span><span>Updated ${new Date(r.pushed_at).toLocaleDateString(undefined,{month:"short",year:"numeric"})}</span></div></a>`).join(""):`<div class="state">No projects match. Clear the search or pick another language.</div>`;
}
$("q").addEventListener("input",renderRepos);
$("chips").addEventListener("click",e=>{const b=e.target.closest(".chip");if(!b)return;activeLang=b.dataset.lang;
  document.querySelectorAll(".chip").forEach(c=>c.setAttribute("aria-pressed",c===b));renderRepos()});

loadStats();loadRepos();
</script>
</body>
</html>

