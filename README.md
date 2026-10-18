<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Gahez — Discover Less. Experience More.</title>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=Sora:wght@700;800&family=JetBrains+Mono:wght@500;700&display=swap" rel="stylesheet">
<style>
:root{--bg:#F7F5FB;--card:#fff;--sub:#ECE9F7;--bd:#DEDBEF;--tx:#14132B;--tx2:#4A4766;--tx3:#8B85B8;--pri:#6C4CF1;--gold:#FFB020;--tan:#FF8A4C;--ok:#2E7D6B;--glow:rgba(108,76,241,.2)}
:root[data-theme=dark]{--bg:#0F0E22;--card:#181735;--sub:#211F45;--bd:#322F5E;--tx:#F7F5FB;--tx2:#B9B4E0;--tx3:#6E6A8C;--glow:rgba(108,76,241,.4)}
*{box-sizing:border-box;margin:0}html{scroll-behavior:smooth}
body{background:var(--bg);color:var(--tx);font:400 16px/1.65 'Space Grotesk',system-ui,sans-serif;overflow-x:hidden;transition:background .4s,color .4s}
h1,h2,h3{letter-spacing:-.02em;line-height:1.1}h1{font-size:clamp(44px,8vw,96px);font-weight:700}h2{font-size:clamp(28px,4vw,48px);font-weight:700;max-width:20ch}h3{font-size:19px;font-weight:600;line-height:1.3}
p{color:var(--tx2);max-width:62ch}.mono{font-family:'JetBrains Mono',monospace}
.w{max-width:1100px;margin:0 auto;padding:0 24px}section{padding:100px 0}.alt{background:var(--sub)}
:focus-visible{outline:3px solid var(--gold);outline-offset:3px}
#bar{position:fixed;top:0;left:0;height:4px;width:0;z-index:70;background:linear-gradient(90deg,var(--pri),var(--gold),var(--tan))}
nav{position:fixed;top:12px;left:50%;transform:translateX(-50%);z-index:60;display:flex;gap:2px;align-items:center;padding:6px;border-radius:99px;background:color-mix(in srgb,var(--card) 72%,transparent);backdrop-filter:blur(16px);border:1px solid var(--bd);max-width:calc(100% - 20px);overflow-x:auto;scrollbar-width:none}
nav a{font:500 12px 'JetBrains Mono',monospace;text-decoration:none;color:var(--tx2);padding:8px 11px;border-radius:99px;transition:.3s}nav a:hover{background:var(--sub)}nav a.on{background:var(--pri);color:#fff}
#tg{border:0;background:var(--gold);color:#14132B;width:34px;height:34px;border-radius:50%;cursor:pointer;flex:none;margin-left:4px}
.lab{font:700 13px 'JetBrains Mono',monospace;color:var(--pri);letter-spacing:.08em;margin-bottom:14px;display:flex;align-items:center;gap:12px}.lab:after{content:'';height:2px;width:60px;background:var(--pri);transform-origin:left;transform:scaleX(0);transition:transform 1s .3s}.in .lab:after,.lab.in:after{transform:none}
/* hero */
.hero{min-height:100vh;display:flex;align-items:center;position:relative;overflow:hidden;padding:120px 0 70px}
.o{position:absolute;border-radius:50%;filter:blur(80px);pointer-events:none;animation:fl 10s ease-in-out infinite}.o1{width:420px;height:420px;background:var(--pri);right:-100px;top:10%;opacity:.5}.o2{width:260px;height:260px;background:var(--gold);left:35%;bottom:5%;opacity:.3;animation-direction:reverse}.o3{width:220px;height:220px;background:var(--tan);left:-60px;top:30%;opacity:.25}
@keyframes fl{50%{transform:translate(-30px,30px) scale(1.08)}}
.hero h1 .wd{display:inline-block;overflow:hidden;vertical-align:bottom}.hero h1 .wd i{display:inline-block;font-style:normal;transform:translateY(110%);animation:up .9s cubic-bezier(.2,.8,.2,1) forwards}
@keyframes up{to{transform:none}}.grad{background:linear-gradient(90deg,var(--pri),var(--tan));-webkit-background-clip:text;background-clip:text;color:transparent}
.hero p.l{font-size:20px;margin:24px 0 30px;animation:fi 1s 1.2s both}@keyframes fi{from{opacity:0;transform:translateY(16px)}}
.chips{display:flex;gap:10px;flex-wrap:wrap}.chip{font-size:13px;font-weight:500;padding:7px 15px;border-radius:99px;background:var(--card);border:1px solid var(--bd);color:var(--tx2);animation:fi .8s both}
.tick{display:flex;gap:6px;margin-top:40px;flex-wrap:wrap;align-items:center;animation:fi 1s 1.6s both}.tick span{font:700 13px 'JetBrains Mono';padding:8px 14px;border-radius:10px;background:var(--card);border:1px solid var(--bd);color:var(--tx3);transition:.4s}.tick span.on{background:var(--pri);color:#fff;border-color:var(--pri);transform:translateY(-6px);box-shadow:0 12px 26px var(--glow)}.tick b{color:var(--tx3)}
/* generic */
.g{display:grid;gap:18px;margin-top:44px}.g2{grid-template-columns:repeat(2,1fr)}.g3{grid-template-columns:repeat(3,1fr)}
.card{background:var(--card);border:1px solid var(--bd);border-radius:22px;padding:26px;position:relative;overflow:hidden;transition:transform .3s,box-shadow .3s}
.card:before{content:'';position:absolute;inset:0;background:radial-gradient(260px circle at var(--mx,50%) var(--my,-50%),var(--glow),transparent);opacity:0;transition:opacity .3s;pointer-events:none}.card:hover:before{opacity:1}.card:hover{transform:translateY(-5px);box-shadow:0 18px 44px var(--glow)}
.card p{margin-top:8px;font-size:15px}.ic{width:44px;height:44px;border-radius:13px;display:grid;place-items:center;background:var(--pri);color:#fff;font:700 15px 'JetBrains Mono';margin-bottom:14px}
.q{border-left:5px solid var(--gold);padding:18px 24px;border-radius:0 18px 18px 0;background:var(--card);margin-top:36px;font-size:20px;font-weight:500;color:var(--tx)}.q b{color:var(--pri)}
.ph{margin-top:36px;border:2px dashed var(--bd);border-radius:20px;padding:26px;color:var(--tx3);display:flex;gap:14px;align-items:center;font-size:14px}.ph:before{content:'+';flex:none;width:34px;height:34px;border-radius:50%;display:grid;place-items:center;background:var(--sub);color:var(--pri);font-weight:700}
.rv{opacity:0;transform:translateY(34px);transition:opacity .8s,transform .8s}.rv.in{opacity:1;transform:none}
/* fragmented */
.sw{display:inline-flex;margin-top:30px;background:var(--card);border:1px solid var(--bd);border-radius:99px;padding:5px}.sw button{font:600 14px inherit;font-family:inherit;border:0;background:none;color:var(--tx2);padding:10px 20px;border-radius:99px;cursor:pointer;transition:.3s}.sw button.on{background:var(--pri);color:#fff}
.fr{position:relative;display:flex;flex-wrap:wrap;gap:14px;justify-content:center;align-items:center;min-height:230px;margin-top:30px;background:var(--card);border:1px solid var(--bd);border-radius:26px;padding:30px}
.fr .c{padding:14px 22px;border-radius:14px;background:var(--sub);border:2px dashed var(--tx3);font-weight:600;transition:all .9s cubic-bezier(.2,.8,.2,1);transform:translate(var(--x),var(--y)) rotate(var(--r))}
.fr.on .c{transform:none;background:var(--pri);color:#fff;border:2px solid var(--pri);box-shadow:0 10px 24px var(--glow)}
.fr .c:nth-child(1){--x:-30px;--y:-26px;--r:-8deg}.fr .c:nth-child(2){--x:40px;--y:30px;--r:6deg}.fr .c:nth-child(3){--x:-40px;--y:34px;--r:9deg}.fr .c:nth-child(4){--x:30px;--y:-30px;--r:-6deg}.fr .c:nth-child(5){--x:-16px;--y:20px;--r:5deg}
.fr .c:nth-child(n+2){transition-delay:calc(var(--d,0)*1s)}
/* tabs */
.tabs{display:flex;gap:10px;flex-wrap:wrap;margin-top:36px}.tb{font:500 15px inherit;font-family:inherit;color:var(--tx2);padding:12px 20px;border-radius:14px;border:1px solid var(--bd);background:var(--card);cursor:pointer;transition:.3s}.tb.on{background:var(--pri);border-color:var(--pri);color:#fff;transform:translateY(-4px);box-shadow:0 12px 28px var(--glow)}
.pn{margin-top:20px;background:var(--card);border:1px solid var(--bd);border-radius:22px;padding:30px;min-height:110px}.pn h3{color:var(--pri);font-size:22px}.pn p{margin-top:8px;animation:fi .5s both}
/* journey */
.jr{display:flex;gap:0;margin-top:44px;position:relative}.jr:before,.jr i{content:'';position:absolute;top:27px;left:5%;height:4px;border-radius:2px}.jr:before{width:90%;background:var(--bd)}.jr i{width:0;background:linear-gradient(90deg,var(--pri),var(--gold),var(--tan));transition:width .7s}
.st{flex:1;text-align:center;background:none;border:0;font:inherit;color:inherit;cursor:pointer;position:relative;z-index:1}.st span{display:grid;place-items:center;width:58px;height:58px;margin:0 auto 10px;border-radius:50%;background:var(--card);border:3px solid var(--bd);font:700 14px 'JetBrains Mono';transition:.4s}.st.on span{background:var(--pri);color:#fff;border-color:var(--pri);box-shadow:0 0 0 8px var(--glow);transform:scale(1.1)}.st.done span{border-color:var(--gold)}.st b{font-size:14px}
/* palette */
.sws{display:grid;grid-template-columns:repeat(5,1fr);gap:12px;margin-top:40px}.sws button{border:0;border-radius:20px;height:140px;color:#fff;text-align:left;padding:14px;display:flex;flex-direction:column;justify-content:flex-end;font:12px 'JetBrains Mono';cursor:pointer;transition:transform .3s}.sws button:hover{transform:translateY(-8px) rotate(-2deg)}.sws b{font:600 14px 'Space Grotesk'}
/* device */
.xp{display:grid;grid-template-columns:.8fr 1.2fr;gap:50px;align-items:center;margin-top:36px}.xt{display:grid;gap:10px}
.xt button{text-align:left;font:inherit;color:inherit;background:var(--card);border:1px solid var(--bd);border-radius:18px;padding:18px 20px;cursor:pointer;transition:.3s}.xt button p{max-height:0;overflow:hidden;margin:0;transition:max-height .4s,margin .4s;font-size:14px}.xt button.on{border-color:var(--pri);box-shadow:0 14px 36px var(--glow);transform:translateX(8px)}.xt button.on p{max-height:140px;margin-top:6px}
.sg{perspective:1400px;display:grid;place-items:center;min-height:620px}
.dev{background:#2a2758;padding:10px;transition:width .6s cubic-bezier(.2,.8,.2,1),aspect-ratio .6s,border-radius .6s,transform .15s;box-shadow:0 40px 80px var(--glow);width:260px;aspect-ratio:390/844;border-radius:42px;overflow:hidden}
.dev[data-k=web]{width:min(100%,560px);aspect-ratio:16/10;border-radius:18px}
.dev .sc{width:100%;height:100%;border-radius:32px;overflow:hidden;background:linear-gradient(145deg,var(--pri),var(--tan));display:grid;place-items:center;color:#fff;font:500 12px 'JetBrains Mono';text-align:center;padding:12px;transition:border-radius .6s}.dev[data-k=web] .sc{border-radius:8px}.dev img{width:100%;height:100%;object-fit:fill;display:block;animation:fi .6s both}
/* quote / foot */
.big{font-size:clamp(26px,4vw,46px);font-weight:700;letter-spacing:-.02em;line-height:1.15;max-width:22ch}
.cta{background:linear-gradient(135deg,var(--pri),#4A2FD1 60%,var(--tan));color:#fff;border-radius:30px;padding:60px 28px;text-align:center;margin-top:50px}.cta p{color:#ECE9F7;margin:12px auto 0}
footer{padding:36px 0;text-align:center;color:var(--tx3);font-size:14px}
@media(max-width:860px){.g3,.g2,.xp{grid-template-columns:1fr}.sws{grid-template-columns:repeat(2,1fr)}.jr{flex-wrap:wrap;gap:18px 0}.jr:before,.jr i{display:none}.st{flex:1 1 33%}section{padding:72px 0}.sg{min-height:560px}.xt button.on{transform:none}}
@media(prefers-reduced-motion:reduce){*{animation:none!important;transition:none!important}.rv,.hero h1 .wd i{opacity:1;transform:none}}
</style>
</head>
<body>
<div id="bar"></div>
<nav id="nv" aria-label="Sections"><button id="tg" aria-label="Toggle dark mode">☾</button></nav>

<header class="hero" id="top"><div class="o o1"></div><div class="o o2"></div><div class="o o3"></div>
<div class="w">
 <div class="chips" style="margin-bottom:26px"><span class="chip" style="animation-delay:.2s">Case study</span><span class="chip" style="animation-delay:.3s">Mobile app &amp; website</span><span class="chip" style="animation-delay:.4s">End-to-end product design</span></div>
 <h1 id="h1" aria-label="Discover less. Experience more."><span class="wd"><i>Discover</i></span> <span class="wd"><i>less.</i></span><br><span class="wd grad"><i>Experience</i></span> <span class="wd grad"><i>more.</i></span></h1>
 <p class="l">A smarter way to discover, plan, and book experiences. Gahez is an event discovery and planning platform that helps people move from “What should we do?” to an actual plan.</p>
 <div class="chips"><span class="chip" style="animation-delay:1.3s">Role: Product Designer — UX/UI, Research, Interaction Design</span><span class="chip" style="animation-delay:1.4s">Tools: Figma, FigJam</span></div>
 <div class="chips" style="margin-top:10px"><span class="chip" style="animation-delay:1.5s">Team: Abrar Ayman · Alaa Ahmed · Mariam Auf · Sherin Ahmed</span></div>
 <div class="tick" id="tick"></div>
</div></header>

<section id="s1"><div class="w"><div class="lab rv">01 · THE PROBLEM</div>
 <h2 class="rv">Planning can feel more complicated than the experience itself</h2>
 <p class="rv" style="margin-top:20px">Finding something enjoyable to do often means switching between platforms to discover events, compare options, coordinate plans, and book tickets. Toggle to see the difference.</p>
 <div class="sw rv" id="sw"><button>Fragmented</button><button class="on">Connected</button></div>
 <div class="fr rv" id="fr"><div class="c">Discover</div><div class="c" style="--d:.1">Compare</div><div class="c" style="--d:.2">Coordinate</div><div class="c" style="--d:.3">Book</div><div class="c" style="--d:.4">Prepare</div></div>
 <div class="q rv"><b>The design challenge:</b> How might we help users discover relevant events and turn their interest into a clear, organized, and bookable plan?</div>
</div></section>

<section class="alt" id="s2"><div class="w"><div class="lab rv">02 · THE GOAL</div>
 <h2 class="rv">One connected experience, from inspiration to attendance</h2>
 <p class="rv" style="margin-top:20px">We designed a connected experience that supports users throughout their event journey. We focused on making it easier to:</p>
 <div class="g g3">
  <div class="card rv"><div class="ic">1</div><h3>Discover</h3><p>Find events that match personal interests.</p></div>
  <div class="card rv"><div class="ic">2</div><h3>Compare</h3><p>Explore and compare options before deciding.</p></div>
  <div class="card rv"><div class="ic">3</div><h3>Organize</h3><p>Shape plans around personal preferences.</p></div>
  <div class="card rv"><div class="ic">4</div><h3>Book</h3><p>Buy tickets through a clear, understandable flow.</p></div>
  <div class="card rv"><div class="ic">5</div><h3>Prepare</h3><p>Access relevant event information before attending.</p></div>
 </div>
</div></section>

<section id="s3"><div class="w"><div class="lab rv">03 · RESEARCH &amp; DISCOVERY</div>
 <h2 class="rv">Understanding how people choose what to do</h2>
 <p class="rv" style="margin-top:20px">Our research explored event-discovery habits, planning challenges, and expectations when choosing activities, informing the journey from discovering an event to committing to a plan.</p>
 <div class="g g2">
  <div class="card rv"><h3>Discovery habits</h3><p>How users currently discover events and activities.</p></div>
  <div class="card rv"><h3>Decision drivers</h3><p>What influences their decisions when comparing options.</p></div>
  <div class="card rv"><h3>Friction points</h3><p>Where friction appears during planning and booking.</p></div>
  <div class="card rv"><h3>Information needs</h3><p>What users need to know before committing to an event.</p></div>
 </div>
 <div class="ph rv">Add your actual survey findings, interview insights, participant count, and supporting evidence here. Include only findings your research supports.</div>
</div></section>

<section class="alt" id="s4"><div class="w"><div class="lab rv">04 · FROM INSIGHTS TO OPPORTUNITIES</div>
 <h2 class="rv">Research observations became design opportunities</h2>
 <div class="tabs rv" id="op"></div><div class="pn rv" id="opp"></div>
 <p class="rv" style="margin-top:22px">These opportunities shaped the information architecture, user flows, and interface decisions.</p>
</div></section>

<section id="s5"><div class="w"><div class="lab rv">05 · STRATEGY &amp; USER JOURNEY</div>
 <h2 class="rv">Discover → Decide → Plan → Book → Prepare → Attend</h2>
 <p class="rv" style="margin-top:20px">Instead of treating discovery and booking as separate activities, the product connects them. The mobile app supports exploring and managing plans, while the website provides a complementary way in. Click a stage.</p>
 <div class="jr rv" id="jr"><i id="jf"></i></div><div class="pn rv" id="jp" style="margin-top:34px"></div>
</div></section>

<section class="alt" id="s6"><div class="w"><div class="lab rv">06 · INFORMATION ARCHITECTURE &amp; FLOWS</div>
 <h2 class="rv">Structured around the tasks users need to complete</h2>
 <p class="rv" style="margin-top:20px">We organized the experience around key tasks, helping users move between discovery, personalization, event details, and planning. The user flows clarified how people move through the product and which screens each step needs.</p>
 <div class="ph rv">Add your information architecture diagram and your most important user flows here.</div>
</div></section>

<section id="s7"><div class="w"><div class="lab rv">07 · VISUAL DESIGN &amp; DESIGN SYSTEM</div>
 <h2 class="rv">A confident purple identity, built to scale</h2>
 <p class="rv" style="margin-top:20px">The visual direction uses a confident purple palette for a recognizable, cohesive identity. The system includes reusable components, typography, color tokens, and interaction states, with light and dark themes. Tap a swatch to copy its hex, or use the moon button to switch themes.</p>
 <div class="sws rv" id="sws"></div>
 <div class="g g3"><div class="card rv"><h3>Consistent across platforms</h3><p>One visual language for the mobile app and the website.</p></div><div class="card rv"><h3>Easy to scale</h3><p>Reusable components and color tokens keep the interface maintainable.</p></div><div class="card rv"><h3>Light and dark</h3><p>Two themes, one product identity.</p></div></div>
</div></section>

<section class="alt" id="s8"><div class="w"><div class="lab rv">08 · THE EXPERIENCE</div>
 <h2 class="rv">Screens with a reason behind each one</h2>
 <div class="xp"><div class="xt rv" id="xt"></div><div class="sg rv" id="sg"><div class="dev" id="dev" data-k="app"><div class="sc" id="sc"></div></div></div></div>
 <p class="mono" style="font-size:12px;color:var(--tx3);margin-top:10px">Move your cursor over the device to tilt it. Place screen files next to this HTML to replace the placeholders.</p>
</div></section>

<section id="s9"><div class="w"><div class="lab rv">09 · DESIGN DECISIONS</div>
 <h2 class="rv">Making the overall journey easier to navigate</h2>
 <div class="g g2">
  <div class="card rv"><div class="ic">↔</div><h3>Connected journeys</h3><p>Link discovery to planning and booking rather than treating each stage independently.</p></div>
  <div class="card rv"><div class="ic">▦</div><h3>Consistent components</h3><p>Reuse design-system elements across screens and platforms.</p></div>
  <div class="card rv"><div class="ic">≡</div><h3>Clear information hierarchy</h3><p>Help users identify relevant event details and available actions.</p></div>
  <div class="card rv"><div class="ic">◐</div><h3>Light and dark themes</h3><p>Offer alternative presentations while keeping the product consistent.</p></div>
 </div>
</div></section>

<section class="alt" id="s10"><div class="w"><div class="lab rv">10 · FINAL OUTCOME</div>
 <h2 class="rv">Discovery, planning and booking in one product</h2>
 <p class="rv" style="margin-top:20px">Gahez brings event discovery, planning, and ticket booking together in one product concept. The project let us explore how strategy, research, interaction design, and a reusable design system work together to support a more connected experience.</p>
 <div class="ph rv">Add validated usability findings, task-completion results, or other measured outcomes here. Don't present unmeasured improvements as proven results.</div>
</div></section>

<section id="s11"><div class="w"><div class="lab rv">11 · REFLECTION</div>
 <h2 class="rv">Designing beyond individual screens</h2>
 <p class="rv" style="margin-top:20px">A useful event platform supports the entire decision-making journey, from helping someone find an idea to giving them the information and tools to act on it. The project also showed the value of a shared design system for a consistent experience across mobile and web.</p>
 <div class="q rv" style="margin-top:40px"><span class="big">Great product design doesn't just help people discover possibilities. It helps them turn those possibilities into action.</span></div>
 <div class="cta rv"><h2 style="margin:0 auto;color:#fff">Designed by Abrar Ayman</h2><p>Product Design · UX Research · Interaction Design · UI Systems</p></div>
</div></section>
<footer>Gahez · Case study</footer>

<script>
const $=s=>document.querySelector(s);
/* nav */
const S=['The Problem','Goal','Research','Insights','Journey','IA & Flows','Design System','Experience','Decisions','Outcome','Reflection'];
S.forEach((n,i)=>{const a=document.createElement('a');a.href='#s'+(i+1);a.textContent=String(i+1).padStart(2,'0');a.title=n;$('#nv').insertBefore(a,$('#tg'))});
const links=[...document.querySelectorAll('nav a')];
const so=new IntersectionObserver(es=>es.forEach(e=>{if(e.isIntersecting)links.forEach(a=>a.classList.toggle('on',a.getAttribute('href')=='#'+e.target.id))}),{rootMargin:'-40% 0px -50% 0px'});
document.querySelectorAll('section[id]').forEach(s=>so.observe(s));
/* hero word delays + journey ticker */
document.querySelectorAll('#h1 i').forEach((e,i)=>e.style.animationDelay=.15*i+.2+'s');
const J=[['Discover','Explore events that match your interests.'],['Decide','Compare options with useful event information.'],['Plan','Organize plans around your preferences.'],['Book','Move through a clear, transparent ticket flow.'],['Prepare','Access the event information you need.'],['Attend','Show up ready, with everything in one place.']];
const tk=$('#tick');J.forEach(([n],i)=>{tk.insertAdjacentHTML('beforeend',`<span>${n}</span>${i<5?'<b>→</b>':''}`)});let ti=0;setInterval(()=>{[...tk.querySelectorAll('span')].forEach((e,k)=>e.classList.toggle('on',k==ti));ti=(ti+1)%6},1100);
/* reveal + glow + progress */
const io=new IntersectionObserver(es=>es.forEach(e=>{if(e.isIntersecting){e.target.classList.add('in');io.unobserve(e.target)}}),{threshold:.12});
document.querySelectorAll('.rv').forEach(e=>io.observe(e));
document.querySelectorAll('.card').forEach(c=>c.addEventListener('pointermove',e=>{const r=c.getBoundingClientRect();c.style.setProperty('--mx',e.clientX-r.left+'px');c.style.setProperty('--my',e.clientY-r.top+'px')}));
addEventListener('scroll',()=>$('#bar').style.width=scrollY/((document.body.scrollHeight-innerHeight))*100+'%',{passive:true});
/* fragmented toggle */
const fr=$('#fr'),sb=[...$('#sw').children];
const setF=on=>{fr.classList.toggle('on',on);sb[0].classList.toggle('on',!on);sb[1].classList.toggle('on',on)};
sb[0].onclick=()=>setF(false);sb[1].onclick=()=>setF(true);setF(false);
new IntersectionObserver((es,o)=>{if(es[0].isIntersecting){setTimeout(()=>setF(true),1500);o.disconnect()}},{threshold:.6}).observe(fr);
/* tabs: opportunities */
const O=[['Discovery','Make exploring events intuitive and engaging.'],['Decision-making','Present useful event information to support comparison.'],['Personalization','Help users find options relevant to their interests.'],['Planning','Connect event discovery with practical next steps.'],['Booking','Keep the ticket-booking journey clear and transparent.']];
const op=$('#op'),opp=$('#opp');
O.forEach(([t,d],i)=>{const b=document.createElement('button');b.className='tb';b.textContent=t;b.onclick=()=>{[...op.children].forEach((e,k)=>e.classList.toggle('on',k==i));opp.innerHTML=`<h3>${t}</h3><p>${d}</p>`};op.appendChild(b)});op.children[0].click();
/* journey */
const jr=$('#jr'),jp=$('#jp');
J.forEach(([n,d],i)=>{const b=document.createElement('button');b.className='st';b.innerHTML=`<span>${i+1}</span><b>${n}</b>`;b.onclick=()=>{[...jr.querySelectorAll('.st')].forEach((e,k)=>{e.classList.toggle('on',k==i);e.classList.toggle('done',k<i)});$('#jf').style.width=(90*i/5)+'%';jp.innerHTML=`<h3>${n}</h3><p>${d}</p>`};jr.appendChild(b)});jr.querySelector('.st').click();
/* palette */
[['Primary violet','#6C4CF1'],['Gold','#FFB020'],['Tangerine','#FF8A4C'],['Success','#2E7D6B'],['Ink','#14132B']].forEach(([n,h])=>{const b=document.createElement('button');b.style.background=h;b.innerHTML=`<b>${n}</b><span>${h}</span>`;b.onclick=()=>{navigator.clipboard&&navigator.clipboard.writeText(h);b.lastChild.textContent='Copied';setTimeout(()=>b.lastChild.textContent=h,1200)};$('#sws').appendChild(b)});
/* experience */
const X=[['Personalization & Discovery','The experience helps users explore activities and events based on their interests, making discovery the starting point for a more relevant journey.',['47___Category_Listing_Template.svg'],'app'],
['Event Details','Event details bring essential information together to help users evaluate an option before deciding whether to proceed.',['Event_Details_1.svg'],'app'],
['Planning & Booking','The product connects the decision to attend with the next steps, reducing the need to manage the process across disconnected experiences.',['Build_My_Weekend.svg'],'app'],
['Mobile & Web','Both platforms share a consistent visual language while each interface supports its own users and tasks.',['Home__hero_section_.svg','Home (hero section).svg'],'web']];
const xt=$('#xt'),dev=$('#dev'),sc=$('#sc');
function show(i){const [t,,f,k]=X[i];[...xt.children].forEach((e,j)=>e.classList.toggle('on',j==i));dev.dataset.k=k;let n=0;const img=new Image();img.alt=t;const nx=()=>{if(n<f.length){img.src=encodeURI(f[n++])}else{sc.textContent=t+' · add '+f[0];}};img.onload=()=>{sc.textContent='';sc.appendChild(img)};img.onerror=nx;sc.textContent='';nx()}
X.forEach(([t,d],i)=>{const b=document.createElement('button');b.innerHTML=`<h3>${t}</h3><p>${d}</p>`;b.onclick=()=>show(i);xt.appendChild(b)});show(0);
$('#sg').addEventListener('pointermove',e=>{const r=$('#sg').getBoundingClientRect();dev.style.transform=`rotateY(${((e.clientX-r.left)/r.width-.5)*28}deg) rotateX(${-((e.clientY-r.top)/r.height-.5)*16}deg)`});
$('#sg').addEventListener('pointerleave',()=>dev.style.transform='');
/* theme */
$('#tg').onclick=()=>{const d=document.documentElement.dataset.theme!='dark';document.documentElement.dataset.theme=d?'dark':'';$('#tg').textContent=d?'☀':'☾'};
</script>
</body>
</html>
