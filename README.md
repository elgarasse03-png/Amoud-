# Amoud-<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>AMOUD | Moroccan Luxury Fragrance</title>

<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;700&family=Poppins:wght@300;400&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
}

body{
font-family:Poppins;
background:black;
color:white;
overflow-x:hidden;
}

/* HERO */

.hero{
height:100vh;
display:flex;
justify-content:center;
align-items:center;
flex-direction:column;
text-align:center;
position:relative;
overflow:hidden;
}

/* VIDEO BACKGROUND */

.hero video{
position:absolute;
top:0;
left:0;
width:100%;
height:100%;
object-fit:cover;
z-index:-1;
filter:brightness(0.35);
}

/* PARTICLES */

.particles{
position:absolute;
width:100%;
height:100%;
background:url("https://www.transparenttextures.com/patterns/dust.png");
opacity:0.25;
animation:particles 25s linear infinite;
}

@keyframes particles{
0%{transform:translateY(0)}
100%{transform:translateY(-600px)}
}

/* PERFUME IMAGE */

.perfume{
width:420px;
max-width:85%;
filter:drop-shadow(0 40px 80px rgba(212,175,55,0.9));
animation:float 6s ease-in-out infinite;
}

@keyframes float{
0%{transform:translateY(0) rotateY(0deg)}
50%{transform:translateY(-10px) rotateY(10deg)}
100%{transform:translateY(0) rotateY(0deg)}
}

/* TITLE */

.title{
font-family:"Playfair Display";
font-size:85px;
letter-spacing:12px;
color:#d4af37;
text-shadow:0 0 30px rgba(212,175,55,0.9);
}

/* TAGLINE */

.tagline{
margin-top:10px;
font-size:20px;
color:#f3d483;
}

/* BUTTON */

.btn{
margin-top:35px;
padding:15px 55px;
border:1px solid #d4af37;
background:transparent;
color:#d4af37;
font-size:18px;
cursor:pointer;
transition:.4s;
}

.btn:hover{
background:#d4af37;
color:black;
box-shadow:0 0 25px gold;
}

/* SECTION */

.section{
padding:120px 20px;
max-width:900px;
margin:auto;
text-align:center;
line-height:1.8;
}

.section h2{
font-family:"Playfair Display";
color:#d4af37;
font-size:38px;
margin-bottom:25px;
}

.section p{
font-size:18px;
opacity:0.9;
}

.ar{
direction:rtl;
margin-top:35px;
font-size:20px;
color:#e9c873;
}

/* VIDEO */

.video{
margin-top:60px;
position:relative;
padding-bottom:56.25%;
height:0;
}

.video iframe{
position:absolute;
top:0;
left:0;
width:100%;
height:100%;
}

/* SCROLL ANIMATION */

.fade{
opacity:0;
transform:translateY(50px);
transition:1.2s;
}

.fade.show{
opacity:1;
transform:translateY(0);
}

/* WHATSAPP FLOAT */

.whatsapp{
position:fixed;
bottom:25px;
right:25px;
background:#25D366;
color:white;
width:60px;
height:60px;
display:flex;
align-items:center;
justify-content:center;
border-radius:50%;
font-size:30px;
text-decoration:none;
box-shadow:0 0 20px rgba(0,0,0,0.5);
}

.whatsapp:hover{
transform:scale(1.1);
}

footer{
text-align:center;
padding:40px;
opacity:0.6;
font-size:14px;
}

</style>
</head>

<body>

<!-- HERO -->

<section class="hero">

<video autoplay muted loop>
<source src="https://streamable.com/2r31cp" type="video/mp4">
</video>

<div class="particles"></div>

<img class="perfume" src="https://i.postimg.cc/QNKzN6cH/Gemini-Generated-Image-l0bnkwl0bnkwl0bn.png">

<div class="title">AMOUD</div>

<div class="tagline">The Essence of Moroccan Luxury</div>

<a href="https://wa.me/212613409601?text=Hello%20I%20want%20AMOUD%20Perfume" target="_blank">

<button class="btn">Discover the Essence</button>

</a>

</section>

<!-- STORY -->

<section class="section fade">

<h2>The Story</h2>

<p>

AMOUD is more than a perfume.

It is a story born from Moroccan nights,

where golden lanterns glow and ancient Amazigh traditions whisper through the air.

Every drop carries mystery, elegance and power.

A fragrance made for those who leave an unforgettable presence.

</p>

<div class="ar">

أمود ليس مجرد عطر...

بل قصة تنبع من ليالي المغرب الدافئة،

حيث تتوهج الفوانيس الذهبية وتهمس التقاليد الأمازيغية القديمة.

كل قطرة تحمل الغموض… والأناقة… والقوة.

</div>

</section>

<!-- VIDEO -->

<section class="section fade">

<h2>Experience AMOUD</h2>

<div class="video">

<iframe src="https://streamable.com/e/2r31cp" frameborder="0" allowfullscreen></iframe>

</div>

</section>

<footer>

AMOUD © Moroccan Luxury Fragrance

</footer>

<a class="whatsapp" href="https://wa.me/212613409601" target="_blank">💬</a>

<script>

const observer=new IntersectionObserver(entries=>{
entries.forEach(entry=>{
if(entry.isIntersecting){
entry.target.classList.add("show")
}
})
})

document.querySelectorAll(".fade").forEach(el=>{
observer.observe(el)
})

</script>

</body>
</html>
