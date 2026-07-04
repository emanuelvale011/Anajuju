<!DOCTYPE html>
<html lang="pt-BR">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Para Anajuju ❤️</title>

<link rel="preconnect" href="https://fonts.googleapis.com">

<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&family=Great+Vibes&display=swap" rel="stylesheet">

<link rel="stylesheet" href="style.css">

</head>

<body>

<div id="loading">

<div class="heart-loader"></div>

<p>Preparando uma surpresa...</p>

</div>

<div id="hearts"></div>

<section id="welcome">

<div class="glass">

<h2>Para a garota mais linda do mundo</h2>

<h1>Anajuju ❤️</h1>

<p>

Se você chegou até aqui...

é porque existe alguém que te ama

mais do que qualquer palavra pode explicar.

</p>

<button id="start">

Clique aqui, meu amor ❤️

</button>

</div>

</section>

<section id="intro" class="hidden">

<div class="intro-box">

<h1 id="typing"></h1>

</div>

</section>

<section id="gallery" class="hidden">

<h1>Nossos Momentos ❤️</h1>

<div class="slider">

<img src="assets/foto1.jpg">

<img src="assets/foto2.jpg">

<img src="assets/foto3.jpg">

<img src="assets/foto4.jpg">

<img src="assets/foto5.jpg">

<img src="assets/foto6.jpg">

<img src="assets/foto7.jpg">

<img src="assets/foto8.jpg">

</div>

</section>

<section id="video" class="hidden">

<h1>Nosso Vídeo ❤️</h1>

<video controls>

<source src="assets/video.mp4" type="video/mp4">

</video>

</section>

<section id="letter" class="hidden">

<div class="paper">

<h1>Para minha Anajuju ❤️</h1>

<p>

Meu amor...

</p>

<p>

Talvez eu nunca consiga encontrar palavras suficientes para mostrar o tamanho do que sinto por você.

</p>

<p>

Você mudou meus dias.

Mudou meu jeito de sorrir.

Mudou meu coração.

</p>

<p>

Quando penso em felicidade...

automaticamente penso em você.

</p>

<p>

Seu sorriso ilumina qualquer momento.

Seu abraço faz qualquer problema desaparecer.

Seu jeitinho faz meu coração bater mais forte todos os dias.

</p>
<p>

Obrigado por existir.

Obrigado por fazer meus dias mais felizes.

Obrigado por ser exatamente quem você é.

</p>

<p>

Eu prometo cuidar de você,
te apoiar,
te fazer sorrir,
e nunca deixar você esquecer
o quanto é especial.

</p>

<p>

Não importa o tempo,
a distância
ou qualquer dificuldade...

Meu coração sempre vai escolher você.

</p>

<p>

Eu te amo hoje.

Vou te amar amanhã.

E vou continuar te amando
todos os dias da minha vida.

</p>

<p class="signature">

❤️ Com todo meu amor,<br>

<b>Emanuel.</b>

</p>

</div>

</section>

<section id="playlist" class="hidden">

<h1>Nossa Playlist 🎵</h1>

<div class="music-list">

<div class="music-card">
🎵 Raindance
</div>

<div class="music-card">
🎵 Always
</div>

<div class="music-card">
🎵 Get You
</div>

<div class="music-card">
🎵 Anna Julia
</div>

<div class="music-card">
🎵 Nights Like This
</div>

<div class="music-card">
🎵 Ivy
</div>

<div class="music-card">
🎵 Best Part
</div>

</div>

</section>

<section id="final" class="hidden">

<div class="final-box">

<h1>

Eu te amo infinitamente,

Anajuju ❤️

</h1>

<p>

Obrigado por ser
a melhor parte da minha vida.

</p>

<h2>

Sempre vou escolher você.

</h2>

</div>

</section>

<canvas id="particles"></canvas>

<script src="script.js"></script>
/* ===========================
   RESET
=========================== */

*{
margin:0;
padding:0;
box-sizing:border-box;
}

html{
scroll-behavior:smooth;
}

body{

font-family:'Poppins',sans-serif;

overflow-x:hidden;

background:linear-gradient(-45deg,
#ff6fa5,
#ff8fb1,
#ffc1d6,
#ffd6e7);

background-size:400% 400%;

animation:bg 15s ease infinite;

color:white;

min-height:100vh;

}

/* ===========================
   FUNDO ANIMADO
=========================== */

@keyframes bg{

0%{

background-position:0% 50%;

}

50%{

background-position:100% 50%;

}

100%{

background-position:0% 50%;

}

}

/* ===========================
   LOADING
=========================== */

#loading{

position:fixed;

width:100%;

height:100vh;

background:#ff7aa9;

display:flex;

flex-direction:column;

justify-content:center;

align-items:center;

z-index:9999;

transition:1s;

}

.heart-loader{

width:60px;

height:60px;

background:#fff;

transform:rotate(45deg);

animation:pulse 1s infinite;

position:relative;

}

.heart-loader::before,
.heart-loader::after{

content:"";

position:absolute;

width:60px;

height:60px;

background:white;

border-radius:50%;

}

.heart-loader::before{

left:-30px;

}

.heart-loader::after{

top:-30px;

}

@keyframes pulse{

0%{

transform:scale(1) rotate(45deg);

}

50%{

transform:scale(1.2) rotate(45deg);

}

100%{

transform:scale(1) rotate(45deg);

}

}

/* ===========================
   TELA INICIAL
=========================== */

#welcome{

height:100vh;

display:flex;

justify-content:center;

align-items:center;

padding:20px;

text-align:center;

}

.glass{

background:rgba(255,255,255,.15);

backdrop-filter:blur(20px);

padding:45px;

border-radius:30px;

box-shadow:0 0 35px rgba(255,255,255,.2);

max-width:700px;

}

.glass h1{

font-family:'Great Vibes',cursive;

font-size:75px;

margin:15px 0;

}

.glass h2{

font-size:20px;

font-weight:400;

}

.glass p{

margin-top:20px;

line-height:1.8;

font-size:18px;

}

button{

margin-top:40px;

padding:18px 40px;

border:none;

border-radius:50px;

background:white;

color:#ff4f8a;

font-size:18px;

font-weight:700;

cursor:pointer;

transition:.4s;

}

button:hover{

transform:scale(1.08);

box-shadow:0 0 25px white
/* ===========================
   INTRO
=========================== */

#intro{

min-height:100vh;

display:flex;

justify-content:center;

align-items:center;

padding:40px;

text-align:center;

}

.intro-box{

max-width:900px;

font-size:30px;

line-height:1.8;

font-weight:600;

}

/* ===========================
   GALERIA
=========================== */

#gallery{

padding:80px 20px;

text-align:center;

}

#gallery h1{

font-size:45px;

margin-bottom:40px;

}

.slider{

display:flex;

gap:25px;

overflow-x:auto;

padding:15px;

scroll-behavior:smooth;

}

.slider::-webkit-scrollbar{

display:none;

}

.slider img{

width:280px;

height:500px;

object-fit:cover;

border-radius:25px;

transition:.4s;

cursor:pointer;

box-shadow:0 10px 30px rgba(0,0,0,.3);

}

.slider img:hover{

transform:scale(1.06);

}

/* ===========================
   VIDEO
=========================== */

#video{

padding:80px 20px;

text-align:center;

}

#video h1{

margin-bottom:30px;

font-size:45px;

}

video{

width:90%;

max-width:900px;

border-radius:25px;

box-shadow:0 15px 35px rgba(0,0,0,.4);

}

/* ===========================
   CARTA
=========================== */

#letter{

padding:100px 25px;

display:flex;

justify-content:center;

}

.paper{

background:white;

color:#444;

padding:50px;

border-radius:30px;

max-width:900px;

box-shadow:0 20px 40px rgba(0,0,0,.25);

line-height:2;

font-size:20px;

}

.paper h1{

color:#ff4d8d;

margin-bottom:30px;

font-family:'Great Vibes',cursive;

font-size:55px;

}

.signature{

margin-top:40px;

text-align:right;

font-size:22px;

}

/* ===========================
   PLAYLIST
=========================== */

#playlist{

padding:90px 20px;

text-align:center;

}

#playlist h1{

font-size:45px;

margin-bottom:40px;

}

.music-list{

display:grid;

grid-template-columns:repeat(auto-fit,minmax(250px,1fr));

gap:25px;

}

.music-card{

background:rgba(255,255,255,.18);

backdrop-filter:blur(15px);

padding:25px;

border-radius:20px;

font-size:22px;

transition:.35s;

cursor:pointer;

}

.music-card:hover{

transform:translateY(-8px);

box-shadow:0 10px 30px rgba(255,255,255,.3);

}

/* ===========================
   FINAL
=========================== */

#final{

height:100vh;

display:flex;

justify-content:center;

align-items:center;

text-align:center;

padding:20px;

}

.final-box h1{

font-family:'Great Vibes',cursive;

font-size:80px;

margin-bottom:25px;

}

.final-box p{

font-size:28px;

margin-bottom:25px;

}

.final-box h2{

font-size:35px;

}

/* ===========================
   RESPONSIVO
=========================== */

@media(max-width:768px){

.glass{

padding:30px;

}

.glass h1{

font-size:55px;

}

.paper{

padding:30px;

font-size:18px;

}

.paper h1{

font-size:42px;

}

.final-box h1{

font-size:55px;

}

.slider img{

width:220px;

height:390px;

}

}
// ==============================
// LOADING
// ==============================

window.addEventListener("load", () => {

setTimeout(() => {

document.getElementById("loading").style.opacity = "0";

setTimeout(() => {

document.getElementById("loading").style.display = "none";

},1000);

},2000);

});

// ==============================
// TELA INICIAL
// ==============================

const start = document.getElementById("start");

const welcome = document.getElementById("welcome");

const intro = document.getElementById("intro");

const gallery = document.getElementById("gallery");

const video = document.getElementById("video");

const letter = document.getElementById("letter");

const playlist = document.getElementById("playlist");

const finalPage = document.getElementById("final");

start.addEventListener("click",()=>{

welcome.style.display="none";

intro.classList.remove("hidden");

typeWriter();

});

// ==============================
// EFEITO MÁQUINA DE ESCREVER
// ==============================

const text = `

Oi, meu amor...

Esse site foi feito especialmente para você.

Quero que sempre que abrir essa página,

você lembre do quanto eu te amo.

Você é a melhor parte dos meus dias.

❤️

`;

let i = 0;

function typeWriter(){

if(i < text.length){

document.getElementById("typing").innerHTML += text.charAt(i);

i++;

setTimeout(typeWriter,55);

}else{

setTimeout(()=>{

gallery.classList.remove("hidden");

video.classList.remove("hidden");

letter.classList.remove("hidden");

playlist.classList.remove("hidden");

finalPage.classList.remove("hidden");

},1000);

}

}

// ==============================
// CORAÇÕES CAINDO
// ==============================

const hearts = document.getElementById("hearts");

function createHeart(){

const heart = document.createElement("div");

heart.innerHTML="❤️";

heart.style.position="fixed";

heart.style.left=Math.random()*100+"vw";

heart.style.top="-30px";

heart.style.fontSize=(20+Math.random()*30)+"px";

heart.style.opacity=Math.random();

heart.style.zIndex="999";

heart.style.pointerEvents="none";

heart.style.animation=`fall ${5+Math.random()*5}s linear`;

document.body.appendChild(heart);

setTimeout(()=>{

heart.remove();

},10000);

}

setInterval(createHeart,350);
// ==============================
// CARROSSEL AUTOMÁTICO
// ==============================

const slider = document.querySelector(".slider");

let direction = 1;

setInterval(() => {

if (!slider) return;

slider.scrollLeft += direction * 320;

if (
slider.scrollLeft + slider.clientWidth >= slider.scrollWidth
) {
direction = -1;
}

if (slider.scrollLeft <= 0) {
direction = 1;
}

}, 2500);

// ==============================
// AMPLIAR FOTO
// ==============================

const imagens = document.querySelectorAll(".slider img");

imagens.forEach((img) => {

img.addEventListener("click", () => {

const fundo = document.createElement("div");

fundo.style.position = "fixed";
fundo.style.left = "0";
fundo.style.top = "0";
fundo.style.width = "100%";
fundo.style.height = "100%";
fundo.style.background = "rgba(0,0,0,.9)";
fundo.style.display = "flex";
fundo.style.justifyContent = "center";
fundo.style.alignItems = "center";
fundo.style.zIndex = "99999";

const foto = document.createElement("img");

foto.src = img.src;

foto.style.maxWidth = "90%";
foto.style.maxHeight = "90%";
foto.style.borderRadius = "20px";
foto.style.boxShadow = "0 0 40px white";

fundo.appendChild(foto);

document.body.appendChild(fundo);

fundo.onclick = () => fundo.remove();

});

});

// ==============================
// PARTÍCULAS
// ==============================

const canvas = document.getElementById("particles");

const ctx = canvas.getContext("2d");

canvas.width = window.innerWidth;
canvas.height = window.innerHeight;

let particles = [];

for (let i = 0; i < 120; i++) {

particles.push({

x: Math.random() * canvas.width,

y: Math.random() * canvas.height,

r: Math.random() * 3 + 1,

dx: (Math.random() - .5),

dy: (Math.random() - .5)

});

}

function animateParticles() {

ctx.clearRect(0,0,canvas.width,canvas.height);

ctx.fillStyle = "rgba(255,255,255,.8)";

particles.forEach(p=>{

ctx.beginPath();

ctx.arc(p.x,p.y,p.r,0,Math.PI*2);

ctx.fill();

p.x += p.dx;

p.y += p.dy;

if(p.x<0)p.x=canvas.width;
if(p.x>canvas.width)p.x=0;
if(p.y<0)p.y=canvas.height;
if(p.y>canvas.height)p.y=0;

});

requestAnimationFrame(animateParticles);

}

animateParticles();

window.addEventListener("resize",()=>{

canvas.width = window.innerWidth;
canvas.height = window.innerHeight;

});

// ==============================
// MENSAGEM FINAL
// ==============================

setInterval(()=>{

const frases=[

"❤️ Eu te amo infinitamente ❤️",

"🌹 Você é meu lugar favorito.",

"✨ Obrigado por existir.",

"💖 Sempre vou escolher você.",

"💕 Você é a melhor parte da minha vida."

];

const frase = frases[Math.floor(Math.random()*frases.length)];

document.title = frase;

},3000);

// ==============================
// CHUVA EXTRA DE CORAÇÕES
// ==============================

function chuvaFinal(){

for(let i=0;i<60;i++){

setTimeout(createHeart,i*120);

}

}

setTimeout(chuvaFinal,15000);

</body>

</html>
