<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Printly</title>
<link rel="preconnect" href="https://fonts.googleapis.com"><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Anton&family=Cairo:wght@400;600;700;800&family=Grand+Hotel&family=Lalezar&display=swap" rel="stylesheet">

<style>
*{box-sizing:border-box}
:root{--mut:#9a9ab8;--panel:#0d0d15}
body{margin:0;font-family:"Cairo","Segoe UI",Tahoma,Arial,sans-serif;color:#fff;min-height:100vh;padding:24px;background:#05050a;overflow-x:hidden}
.bg{position:fixed;inset:0;pointer-events:none;z-index:0;overflow:hidden;
background:radial-gradient(620px 420px at 92% 4%,rgba(124,77,255,.38),transparent 70%),radial-gradient(520px 400px at 4% 42%,rgba(255,47,185,.24),transparent 70%),radial-gradient(640px 420px at 86% 96%,rgba(0,229,255,.24),transparent 70%)}
.bg::before{content:"";position:absolute;inset:0;background:linear-gradient(rgba(255,255,255,.035) 1px,transparent 1px) 0 0/80px 80px,linear-gradient(90deg,rgba(255,255,255,.035) 1px,transparent 1px) 0 0/80px 80px}
.bg svg{position:absolute;top:0;height:100%}
.sq{position:absolute;width:10px;height:10px;box-shadow:0 0 14px currentColor;background:currentColor}
.plus{position:absolute;width:24px;height:24px;opacity:.7}
.plus::before,.plus::after{content:"";position:absolute;background:#fff}
.plus::before{left:11px;top:0;width:1px;height:24px}.plus::after{top:11px;left:0;height:1px;width:24px}
@keyframes bob{50%{transform:translateY(-10px)}}
@keyframes spin{to{transform:rotate(360deg)}}
.wrap{max-width:1050px;margin:auto;position:relative;z-index:1;counter-reset:n}
.hero{position:relative;display:flex;align-items:center;justify-content:center;gap:30px;flex-wrap:wrap;margin:0 0 30px;min-height:250px}
.logo{font-family:"Grand Hotel","Billabong","Lobster",cursive;font-weight:400;direction:ltr;margin:0;line-height:1.15;padding:0 .12em;
font-size:clamp(4.6rem,14vw,8.6rem);background:linear-gradient(90deg,#ff2fb9,#ff9f1c 28%,#ffe14a 45%,#38ff9c 62%,#00e5ff 80%,#7c4dff);
-webkit-background-clip:text;background-clip:text;color:transparent;filter:drop-shadow(0 0 22px rgba(255,47,185,.45))}
.art{filter:drop-shadow(0 0 24px rgba(124,77,255,.55));animation:bob 6s ease-in-out infinite}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(290px,1fr));gap:20px;margin-bottom:20px}
.card{background:linear-gradient(var(--panel),var(--panel)) padding-box,linear-gradient(135deg,var(--c),var(--d,var(--c))) border-box;
border:2px solid transparent;border-radius:30px;padding:22px;box-shadow:0 0 34px -12px var(--c)}
.card h2{margin:0 0 14px;font-family:"Lalezar","Cairo",sans-serif;font-weight:400;font-size:1.6rem;display:flex;align-items:baseline;gap:10px}
.card h2::before{counter-increment:n;content:counter(n,decimal-leading-zero) " —";font-family:"Anton",sans-serif;font-size:1.2rem;color:var(--c);letter-spacing:.04em;direction:ltr}
label{display:block;font-size:.82rem;margin:10px 0 5px;font-weight:600;color:var(--mut)}
input,select{width:100%;padding:10px 13px;border:1px solid #2b2b42;border-radius:14px;font-size:1rem;background:#11111c;font-family:inherit;color:#fff;color-scheme:dark}
input:focus,select:focus{outline:none;border-color:#00e5ff;box-shadow:0 0 0 3px rgba(0,229,255,.2)}
input::placeholder{color:#6b6b8a}
input[type=checkbox]{width:20px;height:20px;accent-color:#ff2fb9;padding:0}
.chk{display:flex;align-items:center;gap:10px;margin-top:14px;font-weight:700;font-size:.95rem;cursor:pointer;color:#fff}
.row{display:flex;gap:10px}.row>div{flex:1}
button{font-family:inherit;border:2px solid transparent;border-radius:999px;padding:10px 20px;font-size:1rem;font-weight:800;color:#fff;background:#0b0b12;cursor:pointer;
display:inline-flex;align-items:center;justify-content:center;gap:10px;transition:transform .15s,box-shadow .2s}
button:hover{transform:translateY(-2px)}
button:disabled{opacity:.4;cursor:not-allowed;transform:none;box-shadow:none}
.b1,.b2{background:linear-gradient(#0b0b12,#0b0b12) padding-box,linear-gradient(90deg,var(--a),var(--b)) border-box}
.b1{--a:#ff2fb9;--b:#ff9f1c}.b2{--a:#7c4dff;--b:#00e5ff}
.b1:hover{box-shadow:0 0 22px rgba(255,47,185,.55)}.b2:hover{box-shadow:0 0 22px rgba(0,229,255,.5)}
.b3{background:#fff;color:#000;padding-block:8px;padding-inline:22px 8px}
.b3::after{content:"←";width:34px;height:34px;border-radius:50%;background:#000;color:#fff;display:grid;place-items:center;font-size:1.1rem}
.b3:hover{box-shadow:0 0 28px rgba(255,255,255,.55)}
.big{width:100%;font-size:1.25rem;margin-top:16px}
.info{margin-top:12px;font-size:.9rem;background:#0a0a12;border:1px dashed #34344f;border-radius:16px;padding:10px 13px;min-height:42px;color:#d6d6ee}
.stats{display:flex;gap:12px;flex-wrap:wrap;margin-bottom:16px}
.chip{flex:1;min-width:130px;text-align:center;padding:14px;border-radius:22px;background:#0a0a12;border:1px solid #2a2a40;color:var(--mut);font-weight:700;font-size:.9rem}
.chip b{display:block;font-family:"Anton","Cairo",sans-serif;font-size:2.3rem;font-weight:400;letter-spacing:.03em;
background:linear-gradient(90deg,var(--a),var(--b));-webkit-background-clip:text;background-clip:text;color:transparent}
.c1{--a:#ff2fb9;--b:#ff9f1c}.c2{--a:#7c4dff;--b:#00b7ff}.c3{--a:#38ff9c;--b:#00e5ff}
.stage{background:linear-gradient(rgba(255,255,255,.05) 1px,transparent 1px) 0 0/28px 28px,linear-gradient(90deg,rgba(255,255,255,.05) 1px,transparent 1px) 0 0/28px 28px,#08080f;
border-radius:24px;padding:22px;text-align:center;border:1px solid #23233a}
#prev{max-width:100%;height:auto;background:#fff;box-shadow:0 0 0 1px #3a3a55,0 0 56px rgba(124,77,255,.5);border-radius:3px}
.nav{display:flex;align-items:center;justify-content:center;gap:14px;margin-bottom:14px}
.nav span{font-family:"Lalezar","Cairo",sans-serif;font-size:1.4rem;min-width:160px;text-align:center;background:linear-gradient(90deg,#ff2fb9,#ff9f1c);-webkit-background-clip:text;background-clip:text;color:transparent}
.dots{display:flex;flex-wrap:wrap;gap:7px;justify-content:center;margin-top:14px}
.dots button{padding:4px 13px;font-size:.85rem;background:#0b0b12;border:1px solid #33334d;color:#cfcfe6}
.dots button.on{background:linear-gradient(90deg,#ff2fb9,#ff9f1c);border-color:transparent;color:#000}
.bar{height:14px;background:#11111c;border:1px solid #2b2b42;border-radius:99px;overflow:hidden;margin-top:16px}
.bar i{display:block;height:100%;width:0;background:linear-gradient(90deg,#ff2fb9,#ff9f1c,#38ff9c,#00e5ff);box-shadow:0 0 14px #00e5ff;transition:width .2s}
#log{margin-top:8px;font-size:.88rem;max-height:120px;overflow:auto;color:var(--mut)}
select option{background:#11111c;color:#fff}
body.locked .wrap{display:none}
#gate{position:fixed;inset:0;z-index:50;display:grid;place-items:center;padding:20px}
.gbox{width:min(400px,100%);text-align:center;background:linear-gradient(#0d0d15,#0d0d15) padding-box,linear-gradient(135deg,var(--c),var(--d)) border-box}
.gbox .logo{font-size:5rem}
.gbox input{text-align:center;margin-top:6px}
#gateMsg{min-height:26px;margin:10px 0 4px;color:#ff5c8a;font-weight:700}
.gbox button{margin:0 auto}
@keyframes shake{25%{transform:translateX(-8px)}75%{transform:translateX(8px)}}
.shake{animation:shake .3s}
</style>
</head>
<body class="locked">
<div class="bg">
<svg style="right:0;width:300px" viewBox="0 0 300 1000" preserveAspectRatio="xMaxYMid slice"><defs>
<linearGradient id="n-l1" x1="0" y1="0" x2="0" y2="1"><stop offset="0" stop-color="#ff2fb9"/><stop offset=".3" stop-color="#ff9f1c"/><stop offset=".55" stop-color="#38ff9c"/><stop offset=".8" stop-color="#00e5ff"/><stop offset="1" stop-color="#7c4dff"/></linearGradient>
<filter id="n-g" x="-50%" y="-10%" width="200%" height="120%"><feGaussianBlur stdDeviation="5" result="b"/><feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge></filter></defs>
<path d="M280 0C280 140 90 190 90 340S270 520 240 700S90 860 150 1000" fill="none" stroke="url(#n-l1)" stroke-width="4" filter="url(#n-g)"/>
<circle cx="90" cy="340" r="7" fill="#fff" filter="url(#n-g)"/><circle cx="240" cy="700" r="7" fill="#fff" filter="url(#n-g)"/></svg>
<svg style="left:0;width:240px" viewBox="0 0 240 1000" preserveAspectRatio="xMinYMid slice">
<path d="M0 120C120 160 200 260 120 400S10 640 130 760S40 940 0 980" fill="none" stroke="url(#n-l1)" stroke-width="3" filter="url(#n-g)" opacity=".85"/></svg>
<i class="sq" style="color:#ff9f1c;top:22%;left:9%"></i><i class="sq" style="color:#7c4dff;top:61%;right:7%"></i><i class="sq" style="color:#ff2fb9;top:84%;left:14%"></i><i class="sq" style="color:#00e5ff;top:11%;right:24%"></i>
<i class="plus" style="top:14%;left:6%"></i><i class="plus" style="top:48%;right:5%"></i><i class="plus" style="top:90%;right:18%"></i>
</div>
<div id="gate"><div class="card gbox" style="--c:#ff2fb9;--d:#7c4dff">
 <h1 class="logo">Printly</h1>
 <label for="gatePass">كلمة السر</label>
 <input type="password" id="gatePass" autocomplete="off" autofocus>
 <div id="gateMsg"></div>
 <button class="b3" id="gateBtn">دخول</button>
</div></div>
<div class="wrap">
<div class="hero">
 <h1 class="logo">Printly</h1>
 <svg class="art" viewBox="0 0 300 260" width="260"><defs>
  <linearGradient id="n-rb" x1="0" y1="0" x2="1" y2="0"><stop offset="0" stop-color="#ff2fb9"/><stop offset=".3" stop-color="#ff9f1c"/><stop offset=".5" stop-color="#ffe14a"/><stop offset=".7" stop-color="#38ff9c"/><stop offset=".85" stop-color="#00e5ff"/><stop offset="1" stop-color="#7c4dff"/></linearGradient>
  <linearGradient id="n-og" x1="0" y1="0" x2="1" y2="1"><stop offset="0" stop-color="#ffc15a"/><stop offset="1" stop-color="#ff5e00"/></linearGradient>
  <linearGradient id="n-pg" x1="0" y1="0" x2="1" y2="1"><stop offset="0" stop-color="#c3a6ff"/><stop offset="1" stop-color="#5b2bff"/></linearGradient>
  <linearGradient id="n-bl" x1="0" y1="0" x2="1" y2="1"><stop offset="0" stop-color="#58b4ff"/><stop offset="1" stop-color="#1b3dff"/></linearGradient></defs>
  <ellipse cx="150" cy="130" rx="142" ry="54" transform="rotate(-24 150 130)" fill="none" stroke="url(#n-rb)" stroke-width="4" filter="url(#n-g)"/>
  <path d="M152 36H202a46 46 0 0 1 0 92H152Z" fill="#2a0f8f" transform="translate(12 -8)"/>
  <path d="M100 52l16-10h40l-16 10z" fill="#ffd9a0"/><path d="M152 52l14-10v178l-14 10z" fill="#c2410c"/>
  <rect x="100" y="52" width="52" height="178" rx="4" fill="url(#n-og)"/>
  <path d="M152 52H202a46 46 0 0 1 0 92H152Z" fill="url(#n-pg)"/><circle cx="197" cy="98" r="17" fill="#05050a"/>
  <rect x="152" y="152" width="46" height="78" rx="5" fill="url(#n-bl)"/>
  <circle cx="126" cy="76" r="4" fill="#05050a" opacity=".55"/><circle cx="126" cy="200" r="4" fill="#05050a" opacity=".55"/><circle cx="175" cy="206" r="4" fill="#05050a" opacity=".55"/>
  <rect x="236" y="40" width="9" height="9" fill="#ff9f1c"/><rect x="40" y="190" width="9" height="9" fill="#00e5ff"/></svg>
</div>
<div class="grid">
 <div class="card" style="--c:#ff3d81;--d:#ff9f1c">
  <h2>اختيار الصور</h2>
  <button class="b1" id="pickImgs" style="width:100%">📁 اختيار مجلد الصور</button>
  <input type="file" id="folderIn" webkitdirectory multiple hidden>
  <input type="file" id="filesIn" accept="image/*" multiple hidden>
  <button class="b1" id="pickFiles" style="width:100%;margin-top:8px;opacity:.85">🖼️ أو اختيار ملفات / صورة واحدة</button>
  <label class="chk"><input type="checkbox" id="rep"> 🔁 تكرار الصورة في الربع كله</label>
  <label>عدد النسخ لكل صورة (اتركه فارغًا لملء ربع كامل)</label>
  <input type="number" id="copies" min="1" placeholder="ملء الربع" disabled>
  <div class="info" id="count">لم يتم اختيار صور بعد</div>
 </div>

 <div class="card" style="--c:#7c4dff;--d:#00b7ff">
  <h2>مقاس الصورة (سم)</h2>
  <div class="row"><div><label>العرض</label><input type="number" id="iw" value="6" step="0.1" min="0.1"></div>
  <div><label>الارتفاع</label><input type="number" id="ih" value="9" step="0.1" min="0.1"></div></div>
  <div class="row"><div><label>المسافة بين الصور</label><input type="number" id="gap" value="0.3" step="0.1" min="0"></div>
  <div><label>هامش الربع</label><input type="number" id="mar" value="0" step="0.1" min="0"></div></div>
  <label>طريقة الملء</label>
  <select id="fit"><option value="cover">ملء كامل مع قص الزيادة</option><option value="contain">احتواء كامل (بدون قص)</option><option value="stretch" selected>تمديد لنفس المقاس</option></select>
 </div>

 
 <div class="card" style="--c:#ff9f1c;--d:#ff2fb9">
  <h2>الترويسة (أعلى كل ربع)</h2>
  <label>اسم العميل</label><input type="text" id="client" placeholder="أدخل اسم العميل">
  <div class="row"><div><label>التاريخ</label><input type="date" id="date"></div>
  <div><label>ارتفاع الترويسة (سم) — 0 لإلغائها</label><input type="number" id="hdr" value="1" step="0.1" min="0"></div></div>
 </div>
</div>

<div class="card" style="--c:#7c4dff;--d:#ff2fb9;margin-bottom:16px">
 <h2>معاينة الأرباع</h2>
 <div class="stats">
  <div class="chip c1"><b id="sPer">–</b>صورة في الربع</div>
  <div class="chip c2"><b id="sGrid">–</b>أعمدة × صفوف</div>
  <div class="chip c3"><b id="sPages">–</b>عدد الأرباع</div>
 </div>
 <div class="nav">
  <button class="b2" id="prevBtn">→ السابق</button>
  <span id="pageLbl">–</span>
  <button class="b2" id="nextBtn">التالي ←</button>
 </div>
 <div class="stage"><canvas id="prev"></canvas></div>
 <div class="dots" id="dots"></div>
</div>

<div class="card" style="--c:#00e5ff;--d:#38ff9c">
 <h2>التحميل</h2>
 <label>شكل الملف الناتج</label>
 <select id="out">
  <option value="jpg">JPG (صورة لكل ربع)</option>
  <option value="png">PNG (صورة لكل ربع)</option>
 </select>
 <label class="chk"><input type="checkbox" id="zip" checked> 🗜️ ضغط الناتج في ملف ZIP واحد</label>
 <div class="row" style="margin-top:12px;align-items:center">
  <div><button class="b2" style="width:100%" id="pickOut">📂 اختيار مكان الحفظ</button></div>
  <div class="info" id="outInfo" style="margin:0;flex:1.4">إن لم تختر مكانًا، سيتم تنزيل الملف عبر المتصفح</div>
 </div>
 <button class="b3 big" id="go" disabled>🚀 ابدأ التجميع والحفظ</button>
 <div class="bar"><i id="bar"></i></div>
 <div id="log"></div>
</div>
</div>

<script>
const $ = id => document.getElementById(id);
let files = [], dirHandle = null, L = {}, items = [], pageCount = 0, cur = 0, tok = 0;
const sleep = ms => new Promise(r => setTimeout(r, ms));
const pad2 = n => String(n).padStart(2, '0');
const t = new Date(); $('date').value = `${t.getFullYear()}-${pad2(t.getMonth()+1)}-${pad2(t.getDate())}`;
const fmtDate = () => { const v = $('date').value; if(!v) return ''; const [y,m,d] = v.split('-'); return `${d}/${m}/${y}`; };

function setFiles(list){
  files = [...list].filter(f => f.type.startsWith('image/')).sort((a,b) => a.name.localeCompare(b.name, undefined, {numeric:true}));
  $('count').textContent = files.length ? `✅ تم اختيار ${files.length} صورة` : 'لم يتم العثور على صور في الاختيار';
  cur = 0; update();
}
$('pickImgs').onclick = () => $('folderIn').click();
$('pickFiles').onclick = () => $('filesIn').click();
$('folderIn').onchange = e => setFiles(e.target.files);
$('filesIn').onchange = e => setFiles(e.target.files);
$('pickOut').onclick = async () => {
  if (!window.showDirectoryPicker) { alert('اختيار مكان الحفظ متاح في متصفحي Chrome وEdge فقط. في المتصفحات الأخرى سيتم تنزيل الملف مباشرة.'); return; }
  try { dirHandle = await window.showDirectoryPicker({mode:'readwrite'}); $('outInfo').textContent = '📂 سيتم الحفظ في: ' + dirHandle.name; } catch(e) {}
};

function calc(){
  const v = id => parseFloat($(id).value) || 0;
  const o = {pw:32, ph:47.5, iw:v('iw'), ih:v('ih'), gap:v('gap'), m:v('mar'), hdr:v('hdr')};
  const aw = o.pw - 2*o.m, ah = o.ph - o.hdr - 2*o.m;
  o.cols = o.iw > 0 ? Math.max(0, Math.floor((aw + o.gap + 1e-9)/(o.iw + o.gap))) : 0;
  o.rows = o.ih > 0 ? Math.max(0, Math.floor((ah + o.gap + 1e-9)/(o.ih + o.gap))) : 0;
  o.ah = ah; return o;
}
function getItems(){
  if (!$('rep').checked) return files.slice();
  const n = parseInt($('copies').value) || (L.cols*L.rows), out = [];
  files.forEach(f => { for (let i=0; i<n; i++) out.push(f); });
  return out;
}

function update(){
  $('copies').disabled = !$('rep').checked;
  L = calc(); items = getItems();
  const per = L.cols*L.rows, ok = per > 0;
  pageCount = ok ? Math.ceil(items.length/per) : 0;
  cur = Math.min(cur, Math.max(0, pageCount-1));
  $('sPer').textContent = per; $('sGrid').textContent = ok ? `${L.cols}×${L.rows}` : '–';
  $('sPages').textContent = pageCount || '–';
  $('go').disabled = !pageCount;
  renderDots(); renderPreview();
}
document.querySelectorAll('input,select').forEach(e => e.addEventListener('input', () => { if(e.type!=='file') update(); }));

function renderDots(){
  const d = $('dots'); d.innerHTML = '';
  if (pageCount < 2 || pageCount > 80) return;
  for (let i=0; i<pageCount; i++){
    const b = document.createElement('button'); b.textContent = i+1; if (i===cur) b.className = 'on';
    b.onclick = () => { cur = i; renderDots(); renderPreview(); }; d.appendChild(b);
  }
}
function go(n){ if (n<0 || n>=pageCount) return; cur = n; renderDots(); renderPreview(); }
$('prevBtn').onclick = () => go(cur-1); $('nextBtn').onclick = () => go(cur+1);
document.addEventListener('keydown', e => {
  if (['INPUT','SELECT'].includes(document.activeElement.tagName)) return;
  if (e.key==='ArrowLeft') go(cur+1); if (e.key==='ArrowRight') go(cur-1);
});

const pcache = new Map();
async function getPrev(file){
  if (pcache.has(file)) return pcache.get(file);
  const b = await createImageBitmap(file, {resizeWidth:300, resizeQuality:'medium'});
  pcache.set(file, b); if (pcache.size > 80) { const k = pcache.keys().next().value; pcache.get(k).close(); pcache.delete(k); }
  return b;
}

function text(g, s, x, y, align){
  g.direction = /[\u0600-\u06FF]/.test(s) ? 'rtl' : 'ltr'; g.textAlign = align; g.fillText(s, x, y);
}
function drawHeader(g, f, p, W){
  if (L.hdr <= 0) return;
  const h = L.hdr*f, pd = Math.max(L.m, 0.5)*f;
  g.fillStyle = '#222'; g.font = `bold ${h*0.5}px "Segoe UI",Tahoma,Arial,sans-serif`; g.textBaseline = 'middle';
  text(g, fmtDate(), pd, h/2, 'left');
  text(g, $('client').value.trim(), W/2, h/2, 'center');
  text(g, `ربع ${p+1} / ${Math.max(1,pageCount)}`, W-pd, h/2, 'right');
  g.strokeStyle = '#888'; g.lineWidth = Math.max(1, f/20);
  g.beginPath(); g.moveTo(pd, h-g.lineWidth); g.lineTo(W-pd, h-g.lineWidth); g.stroke();
}

async function drawPage(g, f, p, mode, cancelled){
  const W = Math.round(L.pw*f), H = Math.round(L.ph*f);
  g.fillStyle = '#fff'; g.fillRect(0,0,W,H); g.imageSmoothingEnabled = true; g.imageSmoothingQuality = 'high';
  drawHeader(g, f, p, W);
  if (!L.cols || !L.rows) return;
  const per = L.cols*L.rows, cw = L.iw*f, ch = L.ih*f, fit = $('fit').value;
  const gw = L.cols*L.iw + (L.cols-1)*L.gap, gh = L.rows*L.ih + (L.rows-1)*L.gap;
  const gx = (L.pw-gw)/2*f, gy = (L.hdr + L.m + (L.ah-gh)/2)*f;
  const pos = i => [gx + (i%L.cols)*(L.iw+L.gap)*f, gy + Math.floor(i/L.cols)*(L.ih+L.gap)*f];
  if (mode === 'prev') {
    g.fillStyle = '#f1eeff'; g.strokeStyle = '#cfc6ff'; g.setLineDash([4,3]); g.lineWidth = 1;
    for (let i=0; i<per; i++){ const [x,y] = pos(i); g.fillRect(x,y,cw,ch); g.strokeRect(x,y,cw,ch); }
    g.setLineDash([]);
  }
  const slice = items.slice(p*per, (p+1)*per), local = new Map();
  for (let i=0; i<slice.length; i++){
    const [x,y] = pos(i); let b = local.get(slice[i]);
    try {
      if (!b) { b = mode === 'prev' ? await getPrev(slice[i]) : await createImageBitmap(slice[i]); local.set(slice[i], b); }
    } catch(e) { continue; }
    if (cancelled && cancelled()) return;
    g.save(); g.beginPath(); g.rect(x,y,cw,ch); g.clip();
    if (fit === 'cover') { const s = Math.max(cw/b.width, ch/b.height), dw = b.width*s, dh = b.height*s; g.drawImage(b, x+(cw-dw)/2, y+(ch-dh)/2, dw, dh); }
    else if (fit === 'contain') { const s = Math.min(cw/b.width, ch/b.height), dw = b.width*s, dh = b.height*s; g.drawImage(b, x+(cw-dw)/2, y+(ch-dh)/2, dw, dh); }
    else g.drawImage(b, x, y, cw, ch);
    g.restore();
  }
  if (mode === 'full') local.forEach(b => b.close());
}

async function renderPreview(){
  const my = ++tok, cv = $('prev');
  const f = Math.min(640/L.ph, 480/L.pw);
  if (!(f > 0) || !isFinite(f)) return;
  cv.width = Math.round(L.pw*f); cv.height = Math.round(L.ph*f);
  $('pageLbl').textContent = pageCount ? `الربع ${cur+1} من ${pageCount}` : 'الربع 1';
  $('prevBtn').disabled = cur <= 0; $('nextBtn').disabled = cur >= pageCount-1;
  await drawPage(cv.getContext('2d'), f, cur, 'prev', () => my !== tok);
}
update();

const logLine = s => { $('log').insertAdjacentHTML('beforeend', `<div>${s}</div>`); $('log').scrollTop = 1e9; };
async function saveBlob(blob, name){
  if (dirHandle) { const fh = await dirHandle.getFileHandle(name, {create:true}); const w = await fh.createWritable(); await w.write(blob); await w.close(); }
  else { const a = document.createElement('a'); a.href = URL.createObjectURL(blob); a.download = name; document.body.appendChild(a); a.click(); a.remove(); setTimeout(() => URL.revokeObjectURL(a.href), 15000); await sleep(600); }
}


const CRC = (() => { const t = new Uint32Array(256); for (let n=0; n<256; n++){ let c = n; for (let k=0; k<8; k++) c = c & 1 ? 0xEDB88320 ^ (c >>> 1) : c >>> 1; t[n] = c >>> 0; } return t; })();
function crc32(u){ let c = 0xFFFFFFFF; for (let i=0; i<u.length; i++) c = CRC[(c ^ u[i]) & 255] ^ (c >>> 8); return (c ^ 0xFFFFFFFF) >>> 0; }
function setJpegDpi(u, dpi){
  const hi = dpi >> 8, lo = dpi & 255;
  if (u[2]===0xFF && u[3]===0xE0 && u[6]===0x4A && u[7]===0x46) { u[13]=1; u[14]=hi; u[15]=lo; u[16]=hi; u[17]=lo; return u; }
  const seg = new Uint8Array([0xFF,0xE0,0,16,0x4A,0x46,0x49,0x46,0,1,1,1,hi,lo,hi,lo,0,0]);
  const out = new Uint8Array(u.length + seg.length); out.set(u.subarray(0,2),0); out.set(seg,2); out.set(u.subarray(2), 2+seg.length); return out;
}
function setPngDpi(u, dpi){
  const ppm = Math.round(dpi/0.0254), ch = new Uint8Array(21), dv = new DataView(ch.buffer);
  dv.setUint32(0, 9); ch.set([0x70,0x48,0x59,0x73], 4); dv.setUint32(8, ppm); dv.setUint32(12, ppm); ch[16] = 1;
  dv.setUint32(17, crc32(ch.subarray(4,17)));
  const out = new Uint8Array(u.length + 21); out.set(u.subarray(0,33)); out.set(ch,33); out.set(u.subarray(33),54); return out;
}
function buildZip(entries){
  const enc = new TextEncoder(), parts = [], central = []; let pos = 0;
  const d = new Date(), dt = ((d.getHours() << 11) | (d.getMinutes() << 5) | (d.getSeconds() >> 1)) & 0xFFFF,
        dd = (((d.getFullYear()-1980) << 9) | ((d.getMonth()+1) << 5) | d.getDate()) & 0xFFFF;
  for (const e of entries){
    const name = enc.encode(e.name), crc = crc32(e.data), size = e.data.length;
    const lh = new DataView(new ArrayBuffer(30));
    lh.setUint32(0, 0x04034b50, true); lh.setUint16(4, 20, true); lh.setUint16(6, 0x0800, true); lh.setUint16(8, 0, true);
    lh.setUint16(10, dt, true); lh.setUint16(12, dd, true); lh.setUint32(14, crc, true); lh.setUint32(18, size, true);
    lh.setUint32(22, size, true); lh.setUint16(26, name.length, true); lh.setUint16(28, 0, true);
    const ch = new DataView(new ArrayBuffer(46));
    ch.setUint32(0, 0x02014b50, true); ch.setUint16(4, 20, true); ch.setUint16(6, 20, true); ch.setUint16(8, 0x0800, true);
    ch.setUint16(10, 0, true); ch.setUint16(12, dt, true); ch.setUint16(14, dd, true); ch.setUint32(16, crc, true);
    ch.setUint32(20, size, true); ch.setUint32(24, size, true); ch.setUint16(28, name.length, true); ch.setUint32(42, pos, true);
    central.push(new Uint8Array(ch.buffer), name);
    parts.push(new Uint8Array(lh.buffer), name, e.data); pos += 30 + name.length + size;
  }
  let cdSize = 0; central.forEach(u => cdSize += u.length);
  const end = new DataView(new ArrayBuffer(22));
  end.setUint32(0, 0x06054b50, true); end.setUint16(8, entries.length, true); end.setUint16(10, entries.length, true);
  end.setUint32(12, cdSize, true); end.setUint32(16, pos, true);
  return new Blob([...parts, ...central, new Uint8Array(end.buffer)], {type:'application/zip'});
}

$('go').onclick = async () => {
  const mode = $('out').value, dpi = 300, f = dpi/2.54;
  const W = Math.round(L.pw*f), H = Math.round(L.ph*f);
  if (W*H > 250e6 || W > 16000 || H > 16000) { alert('مقاس الربع بالبكسل كبير جدًا، يرجى تقليل الدقة DPI.'); return; }
  const q = 1;
  const base = ($('client').value.trim().replace(/[\\/:*?"<>|]/g,'') || 'sheet') + '_' + fmtDate().replace(/\//g,'-');
  const cv = document.createElement('canvas'); cv.width = W; cv.height = H; const g = cv.getContext('2d');
  const total = pageCount, useZip = $('zip').checked, entries = [];
  const emit = async (blob, name) => {
    if (useZip) entries.push({name, data: new Uint8Array(await blob.arrayBuffer())}); else await saveBlob(blob, name);
    logLine(`✅ ${useZip ? 'تمت إضافة' : 'تم حفظ'} ${name}`);
  };
  $('go').disabled = true; $('log').innerHTML = ''; $('bar').style.width = '0';
  try {
    for (let p=0; p<total; p++){
      await drawPage(g, f, p, 'full');
      const png = mode === 'png';
      const blob = await new Promise(r => cv.toBlob(r, png ? 'image/png' : 'image/jpeg', q));
      {
        const raw = new Uint8Array(await blob.arrayBuffer()), data = png ? setPngDpi(raw, dpi) : setJpegDpi(raw, dpi);
        const name = `${base}_ربع_${String(p+1).padStart(3,'0')}.${png?'png':'jpg'}`;
        await emit(new Blob([data], {type: png ? 'image/png' : 'image/jpeg'}), name);
      }
      $('bar').style.width = ((p+1)/total*100) + '%'; await sleep(0);
    }
    if (useZip) {
      const zipName = `${$('client').value.trim().replace(/[\\/:*?"<>|]/g,'') || 'sheet'}_${total}_ربع.zip`;
      await saveBlob(buildZip(entries), zipName); logLine(`📦 تم حفظ الملف المضغوط ${zipName}`);
    }
    logLine('🎉 اكتملت العملية.');
  } catch(e) { logLine('❌ حدث خطأ: ' + e.message); }
  $('go').disabled = false;
};
</script>
<script>
(function(){
  const HASH = '004687553429516cefacdedeaf3a24ce9324d0eb0739c192e21d3ecb883aef5b';
  function sha256(msg){
    const K = [], H = [];
    for (let p=2, c=0; c<64; p++){ let ok = true; for (let i=2; i*i<=p; i++) if (p % i === 0){ ok = false; break; }
      if (ok){ if (c<8) H.push((Math.pow(p,.5) % 1 * 4294967296)|0); K.push((Math.pow(p,1/3) % 1 * 4294967296)|0); c++; } }
    const b = [...new TextEncoder().encode(msg)], l = b.length*8; b.push(0x80);
    while (b.length % 64 !== 56) b.push(0);
    for (let i=7; i>=0; i--) b.push(i>3 ? 0 : (l >>> (i*8)) & 255);
    const rr = (x,n) => (x>>>n) | (x<<(32-n)); let h = H.slice();
    for (let o=0; o<b.length; o+=64){
      const w = new Array(64);
      for (let i=0; i<16; i++) w[i] = (b[o+4*i]<<24)|(b[o+4*i+1]<<16)|(b[o+4*i+2]<<8)|b[o+4*i+3];
      for (let i=16; i<64; i++){ const s0 = rr(w[i-15],7)^rr(w[i-15],18)^(w[i-15]>>>3), s1 = rr(w[i-2],17)^rr(w[i-2],19)^(w[i-2]>>>10); w[i] = (w[i-16]+s0+w[i-7]+s1)|0; }
      let [a,bb,c,d,e,f,g,hh] = h;
      for (let i=0; i<64; i++){
        const S1 = rr(e,6)^rr(e,11)^rr(e,25), ch = (e&f)^(~e&g), t1 = (hh+S1+ch+K[i]+w[i])|0;
        const S0 = rr(a,2)^rr(a,13)^rr(a,22), mj = (a&bb)^(a&c)^(bb&c), t2 = (S0+mj)|0;
        hh = g; g = f; f = e; e = (d+t1)|0; d = c; c = bb; bb = a; a = (t1+t2)|0;
      }
      h = [h[0]+a,h[1]+bb,h[2]+c,h[3]+d,h[4]+e,h[5]+f,h[6]+g,h[7]+hh].map(x => x|0);
    }
    return h.map(x => (x>>>0).toString(16).padStart(8,'0')).join('');
  }
  const gate = document.getElementById('gate'), inp = document.getElementById('gatePass'), msg = document.getElementById('gateMsg');
  const unlock = () => { document.body.classList.remove('locked'); gate.remove(); try { sessionStorage.setItem('printly_ok','1'); } catch(e) {} };
  let ok = false; try { ok = sessionStorage.getItem('printly_ok') === '1'; } catch(e) {}
  if (ok) { unlock(); return; }
  const check = () => {
    if (sha256(inp.value.trim()) === HASH) unlock();
    else { msg.textContent = 'كلمة السر غير صحيحة'; const bx = gate.firstElementChild; bx.classList.remove('shake'); void bx.offsetWidth; bx.classList.add('shake'); inp.select(); }
  };
  document.getElementById('gateBtn').onclick = check;
  inp.addEventListener('keydown', e => { if (e.key === 'Enter') check(); });
  inp.focus();
})();
</script>
</body>
</html>
