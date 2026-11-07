# Charlie-krik
Fun
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>HEY CHARLIE KIRK CLICKER</title>
<style>
*{box-sizing:border-box}
body{margin:0;background:radial-gradient(circle at top,#39234f,#10101b 65%);color:white;font-family:Arial,sans-serif;text-align:center;padding:20px}
h1{color:#ffd35b;font-size:clamp(28px,6vw,48px);text-shadow:0 0 25px #ffae24}
.panel{max-width:650px;margin:16px auto;padding:20px;background:#ffffff0c;border:1px solid #ffffff25;border-radius:20px}
.stats{display:grid;grid-template-columns:repeat(3,1fr);gap:10px}
.stat{background:#ffffff12;padding:14px;border-radius:12px}
.stat b{display:block;font-size:23px;color:#ffd35b;margin-top:8px}
#clicker{width:210px;height:210px;border-radius:50%;border:6px solid #ffe18a;background:radial-gradient(circle at 35% 25%,#fff3a6,#ffb52c 45%,#8e4200);color:#351900;font-size:24px;font-weight:1000;box-shadow:0 0 40px #ffb52c88;cursor:pointer;transition:.1s;animation:glow 2s infinite}
#clicker:active{transform:scale(.91)}
@keyframes glow{50%{box-shadow:0 0 65px #ffb52c}}
button{cursor:pointer}
.shop{display:grid;gap:10px}
.upgrade{display:flex;align-items:center;text-align:left;gap:12px;width:100%;padding:13px;background:#ffffff12;border:1px solid #ffffff25;color:white;border-radius:12px}
.upgrade:disabled{opacity:.35;cursor:not-allowed}
.upgrade .info{flex:1}
.upgrade strong{color:#ffd35b}
.small{font-size:12px;color:#aaa;margin-top:5px}
.tabs{display:flex;justify-content:center;gap:8px;flex-wrap:wrap}
.tabs button,.control{background:#e4a92f;color:#271700;border:0;border-radius:9px;padding:10px 14px;font-weight:bold}
.tabs button.active{background:#fff0a2}
.hidden{display:none!important}
#message{color:#ffe18a;min-height:25px;margin-top:15px;font-weight:bold}
.achievement{padding:12px;background:#ffffff12;border-radius:10px;text-align:left}
.locked{opacity:.35}
#trophies{display:grid;grid-template-columns:1fr 1fr;gap:10px}
.bar{height:9px;background:#ffffff22;border-radius:10px;overflow:hidden;margin-top:8px}
#progress{height:100%;width:0;background:#ffcb4c}
#floaters{position:relative;height:0}
.float{position:absolute;left:50%;top:-100px;color:#ffe18a;font-weight:bold;font-size:23px;animation:float .8s forwards;pointer-events:none}
@keyframes float{to{opacity:0;transform:translateY(-100px) translateX(30px)}}
</style>
</head>
<body>
<h1>🎤 HEY CHARLIE KIRK!</h1>
<p>THE ULTIMATE CLICKER GAME</p>

<div class="panel">
<div class="stats">
<div class="stat">COINS<b id="coins">0</b></div>
<div class="stat">PER CLICK<b id="power">1</b></div>
<div class="stat">PER SECOND<b id="cps">0</b></div>
</div>
</div>

<div class="panel">
<p>👆 TAP THE BUTTON!</p>
<div id="floaters"></div>
<button id="clicker">🎤<br>HEY CHARLIE!</button>
<div id="message">Let's get clicking!</div>
<br>
<button class="control" id="sound">🔊 SOUND ON</button>
<button class="control" id="bonus">🎁 DAILY BONUS</button>
</div>

<div class="panel">
<h3 id="level">LEVEL 1</h3>
<p>PROGRESSION</p>
<div class="bar"><div id="progress"></div></div>
<p id="progressText">0 / 100</p>
</div>

<div class="panel">
<div class="tabs">
<button class="active" data-tab="shop">🛒 SHOP</button>
<button data-tab="achievements">🏆 TROPHIES</button>
<button data-tab="statistics">📊 STATS</button>
</div>
</div>

<div class="panel" id="shop">
<h2>⚡ UPGRADE SHOP</h2>
<div class="shop" id="upgrades"></div>
</div>

<div class="panel hidden" id="achievements">
<h2>🏆 ACHIEVEMENTS</h2>
<div id="trophies"></div>
</div>

<div class="panel hidden" id="statistics">
<h2>📊 YOUR STATS</h2>
<div id="stats"></div>
<button class="control" id="reset" style="background:#a32e38;color:white;margin-top:20px">RESET GAME</button>
</div>

<p style="color:#888;font-size:12px">UNOFFICIAL FAN-MADE PARODY GAME</p>

<script>
const $=id=>document.getElementById(id);

const upgrades=[
{name:"Louder Microphone",icon:"🎤",desc:"+1 per click",cost:25,type:"power",amount:1},
{name:"Podcast Studio",icon:"🎙️",desc:"+2 per second",cost:80,type:"auto",amount:2},
{name:"Mega Megaphone",icon:"📢",desc:"+5 per click",cost:250,type:"power",amount:5},
{name:"Camera Crew",icon:"📹",desc:"+10 per second",cost:500,type:"auto",amount:10},
{name:"Viral Clip Factory",icon:"📱",desc:"+25 per second",cost:1600,type:"auto",amount:25},
{name:"Golden Microphone",icon:"🥇",desc:"+30 per click",cost:2500,type:"power",amount:30},
{name:"Meme Empire",icon:"👑",desc:"+100 per second",cost:10000,type:"auto",amount:100},
{name:"Supercomputer",icon:"🖥️",desc:"DOUBLE click power",cost:25000,type:"mult",amount:2},
{name:"Infinite Podcast",icon:"♾️",desc:"+500 per second",cost:75000,type:"auto",amount:500},
{name:"CLICKING MACHINE",icon:"🚀",desc:"TRIPLE click power",cost:200000,type:"mult",amount:3}
];

const achievements=[
["First Click","Make your first click",s=>s.clicks>=1],
["Getting Started","Earn 100 coins",s=>s.total>=100],
["Click Addict","Make 100 clicks",s=>s.clicks>=100],
["Pocket Change","Earn 1,000 coins",s=>s.total>=1000],
["Going Viral","Earn 10,000 coins",s=>s.total>=10000],
["Influencer","Make 1,000 clicks",s=>s.clicks>=1000],
["Millionaire","Earn 1 million coins",s=>s.total>=1000000],
["Absolute Legend","Earn 10 million coins",s=>s.total>=10000000]
];

let s={
coins:0,total:0,clicks:0,items:Array(10).fill(0),
mult:1,level:1,sound:true,bonus:false,earned:[]
};

try{
let saved=JSON.parse(localStorage.getItem("charlie_clicker"));
if(saved&&Array.isArray(saved.items)&&saved.items.length===10)
s={...s,...saved};
}catch(e){}

let audio;

function fmt(n){
if(n>=1e12)return(n/1e12).toFixed(2)+"T";
if(n>=1e9)return(n/1e9).toFixed(2)+"B";
if(n>=1e6)return(n/1e6).toFixed(2)+"M";
if(n>=10000)return(n/1000).toFixed(1)+"K";
return Math.floor(n).toLocaleString();
}

function clickPower(){
return (1+upgrades.reduce((a,u,i)=>a+(u.type==="power"?u.amount*s.items[i]:0),0))*s.mult;
}

function income(){
return upgrades.reduce((a,u,i)=>a+(u.type==="auto"?u.amount*s.items[i]:0),0);
}

function price(i){
return Math.floor(upgrades[i].cost*Math.pow(1.48,s.items[i]));
}

function save(){
try{localStorage.setItem("charlie_clicker",JSON.stringify(s))}catch(e){}
}

function tone(freq=500,duration=.1){
if(!s.sound)return;
try{
audio=audio||new(window.AudioContext||window.webkitAudioContext)();
if(audio.state==="suspended")audio.resume();
let o=audio.createOscillator();
let g=audio.createGain();
o.frequency.value=freq;
o.type="triangle";
g.gain.setValueAtTime(.06,audio.currentTime);
g.gain.exponentialRampToValueAtTime(.001,audio.currentTime+duration);
o.connect(g);g.connect(audio.destination);
o.start();o.stop(audio.currentTime+duration);
}catch(e){}
}

function earn(n){
s.coins+=n;
s.total+=n;
}

function floatText(text){
let f=document.createElement("div");
f.className="float";
f.textContent=text;
$("floaters").appendChild(f);
setTimeout(()=>f.remove(),850);
}

function click(){
let crit=Math.random()<.055;
let amount=clickPower()*(crit?5:1);
earn(amount);
s.clicks++;
floatText((crit?"⭐ CRITICAL! +":"+")+fmt(amount));
tone(crit?950:550);
$("message").textContent=crit?"🔥 FIVE TIMES THE COINS!":"HEY CHARLIE!";
update();
}

function buy(i){
let p=price(i);
if(s.coins<p)return;
s.coins-=p;
s.items[i]++;
if(upgrades[i].type==="mult")s.mult*=upgrades[i].amount;
tone(700);
setTimeout(()=>tone(950),100);
$("message").textContent=upgrades[i].name+" PURCHASED!";
update();
}

function update(){
$("coins").textContent=fmt(s.coins);
$("power").textContent=fmt(clickPower());
$("cps").textContent=fmt(income());

let need=s.level*100;
let progress=s.total%need;
$("level").textContent="⭐ LEVEL "+s.level;
$("progress").style.width=progress/need*100+"%";
$("progressText").textContent=fmt(progress)+" / "+fmt(need);

$("upgrades").innerHTML=upgrades.map((u,i)=>{
let p=price(i);
return `<button class="upgrade" data-buy="${i}" ${s.coins<p?"disabled":""}>
<span style="font-size:27px">${u.icon}</span>
<span class="info"><strong>${u.name}</strong> ×${s.items[i]}<div class="small">${u.desc}</div></span>
<span>🪙 ${fmt(p)}</span>
</button>`;
}).join("");

$("trophies").innerHTML=achievements.map(([name,desc,fn])=>{
let won=fn(s);
if(won&&!s.earned.includes(name)){
s.earned.push(name);
tone(900);
}
return `<div class="achievement ${won?"":"locked"}">
<div style="font-size:22px">${won?"🏆":"🔒"}</div>
<strong>${name}</strong>
<div class="small">${desc}</div>
</div>`;
}).join("");

$("stats").innerHTML=[
["Total clicks",fmt(s.clicks)],
["Lifetime coins",fmt(s.total)],
["Coins per click",fmt(clickPower())],
["Coins per second",fmt(income())],
["Upgrades purchased",s.items.reduce((a,b)=>a+b,0)],
["Achievements",s.earned.length+"/"+achievements.length]
].map(([a,b])=>`<div class="stat" style="margin:7px">${a}<b>${b}</b></div>`).join("");

save();
}

$("clicker").onclick=click;

$("upgrades").onclick=e=>{
let b=e.target.closest("[data-buy]");
if(b)buy(+b.dataset.buy);
};

document.querySelectorAll("[data-tab]").forEach(b=>{
b.onclick=()=>{
document.querySelectorAll("[data-tab]").forEach(x=>x.classList.toggle("active",x===b));
["shop","achievements","statistics"].forEach(id=>{
$(id).classList.toggle("hidden",id!==b.dataset.tab);
});
};
});

$("sound").onclick=()=>{
s.sound=!s.sound;
$("sound").textContent=s.sound?"🔊 SOUND ON":"🔇 SOUND OFF";
if(s.sound)tone(700);
save();
};

$("bonus").onclick=()=>{
if(s.bonus){
$("message").textContent="You've already collected your bonus!";
return;
}
s.bonus=true;
let amount=Math.max(100,Math.floor(s.total*.2+100));
earn(amount);
tone(800,.2);
$("message").textContent="🎁 BONUS: +"+fmt(amount)+" COINS!";
update();
};

$("reset").onclick=()=>{
if(confirm("Delete ALL progress?")){
localStorage.removeItem("charlie_clicker");
s={coins:0,total:0,clicks:0,items:Array(10).fill(0),mult:1,level:1,sound:true,bonus:false,earned:[]};
update();
}
};

setInterval(()=>{
if(income()>0){
earn(income()/10);
update();
}
},100);

setInterval(()=>{
let level=1;
while(s.total>=level*100)level++;
if(level>s.level){
s.level=level;
tone(600,.2);
$("message").textContent="⭐ LEVEL UP! LEVEL "+level;
update();
}
},500);

update();
</script>
</body>
</html>
