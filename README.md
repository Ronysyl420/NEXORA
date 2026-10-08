<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>NEXORA ($NEXO) — Born From Nothing</title>

<meta name="description"
content="NEXORA ($NEXO) — Born From Nothing. Built By Everyone. A community-driven meme coin on Solana.">

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family:Arial,Helvetica,sans-serif;
    background:#050509;
    color:#fff;
    line-height:1.6;
    overflow-x:hidden;
}

/* NAVBAR */
nav{
    position:fixed;
    top:0;
    width:100%;
    padding:16px 7%;
    display:flex;
    justify-content:space-between;
    align-items:center;
    background:rgba(5,5,9,.88);
    backdrop-filter:blur(15px);
    z-index:1000;
    border-bottom:1px solid rgba(139,92,246,.2);
}

.logo{
    font-size:25px;
    font-weight:900;
    letter-spacing:2px;
}

.logo span{
    color:#8b5cf6;
}

nav a{
    color:#fff;
    text-decoration:none;
    margin-left:25px;
    font-size:14px;
    transition:.3s;
}

nav a:hover{
    color:#a78bfa;
}

/* HERO */
.hero{
    min-height:100vh;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    padding:120px 20px 70px;

    background:
    radial-gradient(circle at 50% 20%,rgba(139,92,246,.28),transparent 35%),
    radial-gradient(circle at 20% 80%,rgba(0,200,255,.12),transparent 30%),
    #050509;
}

.hero-content{
    max-width:900px;
}

.tagline{
    font-size:14px;
    letter-spacing:4px;
    text-transform:uppercase;
    color:#a78bfa;
    margin-bottom:15px;
}

.hero-image{
    width:min(430px,85vw);
    margin:10px auto 25px;
    display:block;
    border-radius:50%;
    filter:
        drop-shadow(0 0 15px rgba(139,92,246,.6))
        drop-shadow(0 0 45px rgba(0,180,255,.25));
    animation:float 4s ease-in-out infinite;
}

@keyframes float{
    0%,100%{
        transform:translateY(0);
    }
    50%{
        transform:translateY(-10px);
    }
}

.hero h1{
    font-size:clamp(55px,12vw,110px);
    font-weight:1000;
    letter-spacing:-5px;
    line-height:1;
}

.hero h1 span{
    color:#8b5cf6;
}

.hero p{
    max-width:680px;
    margin:18px auto;
    color:#b8b8c7;
    font-size:18px;
}

.hero-sub{
    font-size:15px !important;
    color:#8f8fa3 !important;
}

.buttons{
    margin-top:30px;
}

.btn{
    display:inline-block;
    padding:14px 27px;
    margin:7px;
    border-radius:30px;
    text-decoration:none;
    color:#fff;
    font-weight:bold;
    border:1px solid #8b5cf6;
    transition:.3s;
}

.btn.primary{
    background:linear-gradient(135deg,#8b5cf6,#6366f1);
    box-shadow:0 0 20px rgba(139,92,246,.25);
}

.btn:hover{
    transform:translateY(-4px);
    box-shadow:0 0 30px rgba(139,92,246,.5);
}

/* SECTIONS */
section{
    padding:90px 7%;
}

.title{
    text-align:center;
    margin-bottom:45px;
}

.title h2{
    font-size:40px;
    margin-bottom:8px;
}

.title p{
    color:#9999aa;
}

/* CARDS */
.grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
    gap:20px;
    max-width:1100px;
    margin:auto;
}

.card{
    background:
        linear-gradient(145deg,rgba(139,92,246,.08),rgba(255,255,255,.02));
    border:1px solid rgba(255,255,255,.08);
    padding:28px;
    border-radius:20px;
    transition:.3s;
}

.card:hover{
    transform:translateY(-6px);
    border-color:rgba(139,92,246,.5);
    box-shadow:0 10px 35px rgba(0,0,0,.3);
}

.card h3{
    margin-bottom:10px;
}

.card p{
    color:#aaaabb;
}

.big{
    font-size:27px;
    font-weight:bold;
    color:#a78bfa;
}

/* CONTRACT */
.contract{
    max-width:850px;
    margin:30px auto;
    padding:22px;
    border-radius:15px;
    background:#0d0d15;
    border:1px dashed #8b5cf6;
    text-align:center;
    word-break:break-all;
    color:#aaa;
}

.contract strong{
    color:#a78bfa;
    font-size:20px;
}

/* ROADMAP */
.roadmap{
    max-width:850px;
    margin:auto;
}

.step{
    margin-bottom:20px;
    padding:25px;
    border-left:3px solid #8b5cf6;
    background:#0d0d15;
    border-radius:0 15px 15px 0;
    transition:.3s;
}

.step:hover{
    transform:translateX(5px);
    background:#10101b;
}

.step h3{
    color:#a78bfa;
    margin-bottom:8px;
}

.step p{
    color:#aaaabb;
}

/* COMMUNITY */
.community-box{
    max-width:850px;
    margin:auto;
    text-align:center;
    padding:45px 20px;
    background:
        radial-gradient(circle at center,rgba(139,92,246,.15),transparent 60%),
        #0d0d15;
    border:1px solid rgba(139,92,246,.2);
    border-radius:25px;
}

.social{
    margin:25px 0;
}

.social a{
    display:inline-block;
    color:#a78bfa;
    margin:8px 12px;
    text-decoration:none;
    font-weight:bold;
}

.social a:hover{
    color:#fff;
}

/* FOOTER */
footer{
    text-align:center;
    padding:40px 20px;
    border-top:1px solid rgba(255,255,255,.08);
    color:#777;
}

footer p{
    margin:6px;
}

/* MOBILE */
@media(max-width:600px){

    nav{
        padding:15px 5%;
    }

    nav a{
        display:none;
    }

    .hero{
        padding-top:100px;
    }

    .hero-image{
        width:280px;
    }

    .hero h1{
        font-size:65px;
        letter-spacing:-3px;
    }

    .hero p{
        font-size:16px;
    }

    section{
        padding:70px 5%;
    }

    .title h2{
        font-size:32px;
    }

    .card{
        padding:23px;
    }
}
</style>
</head>

<body>

<!-- NAVIGATION -->
<nav>

<div class="logo">
NEX<span>ORA</span>
</div>

<div>
<a href="#about">About</a>
<a href="#tokenomics">Tokenomics</a>
<a href="#roadmap">Roadmap</a>
<a href="#community">Community</a>
</div>

</nav>


<!-- HERO -->
<section class="hero">

<div class="hero-content">

<div class="tagline">
SOLANA COMMUNITY MEME COIN
</div>

<img
class="hero-image"
src="file_00000000f8a88211ac8145c625d3b8f1.png"
alt="NEXORA $NEXO">

<h1>
NEX<span>ORA</span>
</h1>

<p>
Born From Nothing.<br>
Built By Everyone.
</p>

<p class="hero-sub">
A community-driven meme movement on Solana.
<br>
No promises. Just memes, community and ambition.
</p>

<div class="buttons">

<a class="btn primary" href="#tokenomics">
EXPLORE $NEXO
</a>

<a class="btn" href="#community">
JOIN COMMUNITY
</a>

</div>

</div>

</section>


<!-- ABOUT -->
<section id="about">

<div class="title">

<h2>What is NEXORA?</h2>

<p>The meme starts here.</p>

</div>

<div class="grid">

<div class="card">

<h3>🌌 Community</h3>

<p>
NEXORA is built around its community.
Everyone can become part of the movement.
</p>

</div>


<div class="card">

<h3>🚀 Solana</h3>

<p>
NEXORA is designed around the fast and low-cost
Solana ecosystem.
</p>

</div>


<div class="card">

<h3>🔥 Meme Culture</h3>

<p>
Memes, creativity and community are the heart
of NEXORA.
</p>

</div>

</div>

</section>


<!-- TOKENOMICS -->
<section id="tokenomics">

<div class="title">

<h2>Tokenomics</h2>

<p>Simple. Transparent. Community focused.</p>

</div>

<div class="grid">

<div class="card">

<h3>Total Supply</h3>

<div class="big">
1,000,000,000
</div>

<p>$NEXO</p>

</div>


<div class="card">

<h3>Liquidity</h3>

<div class="big">
60%
</div>

<p>Planned allocation</p>

</div>


<div class="card">

<h3>Community</h3>

<div class="big">
15%
</div>

<p>Airdrops & rewards</p>

</div>


<div class="card">

<h3>Marketing</h3>

<div class="big">
10%
</div>

<p>Community growth</p>

</div>


<div class="card">

<h3>Development</h3>

<div class="big">
5%
</div>

<p>Project development</p>

</div>


<div class="card">

<h3>Reserve</h3>

<div class="big">
10%
</div>

<p>Future ecosystem needs</p>

</div>

</div>

</section>


<!-- CONTRACT -->
<section>

<div class="title">

<h2>Contract</h2>

<p>Official $NEXO contract information.</p>

</div>

<div class="contract">

<strong>COMING SOON</strong>

<br><br>

Official Solana contract address will be published
after token deployment.

</div>

</section>


<!-- ROADMAP -->
<section id="roadmap">

<div class="title">

<h2>Roadmap</h2>

<p>From zero to NEXORA.</p>

</div>

<div class="roadmap">

<div class="step">

<h3>PHASE 01 — GENESIS</h3>

<p>
Brand creation, website launch, community setup
and social media presence.
</p>

</div>


<div class="step">

<h3>PHASE 02 — LAUNCH</h3>

<p>
Token deployment, liquidity setup and
initial community distribution.
</p>

</div>


<div class="step">

<h3>PHASE 03 — EXPANSION</h3>

<p>
Community campaigns, partnerships,
creator collaborations and ecosystem growth.
</p>

</div>


<div class="step">

<h3>PHASE 04 — NEXORA</h3>

<p>
Build a recognizable meme community
and continue developing the ecosystem.
</p>

</div>

</div>

</section>


<!-- COMMUNITY -->
<section id="community">

<div class="community-box">

<div class="title">

<h2>Join NEXORA</h2>

<p>Be part of the beginning.</p>

</div>

<div class="social">

<!-- এখানে তোমার আসল X link বসাবে -->
<a href="#" target="_blank">𝕏 X / Twitter</a>

<!-- এখানে Telegram link বসাবে -->
<a href="#" target="_blank">✈ Telegram</a>

<!-- এখানে Discord link বসাবে -->
<a href="#" target="_blank">💬 Discord</a>

</div>

<a class="btn primary" href="#">
JOIN THE MOVEMENT
</a>

</div>

</section>


<!-- FOOTER -->
<footer>

<p>
© 2026 NEXORA. All rights reserved.
</p>

<p>
NEXORA is a meme/community project.
Nothing on this website constitutes financial advice.
</p>

</footer>

</body>
</html>
