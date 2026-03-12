
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>CozyCup Coffee</title>

<style>

@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap');

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
scroll-behavior:smooth;
}

body{
background:#f5eee7;
color:#3d2b1f;
}

/* NAVBAR */

nav{
position:fixed;
top:0;
width:100%;
display:flex;
justify-content:space-between;
align-items:center;
padding:15px 8%;
background:rgba(92,58,46,0.85);
backdrop-filter:blur(10px);
color:white;
z-index:1000;
}

.logo{
font-size:24px;
font-weight:600;
}

nav ul{
display:flex;
list-style:none;
gap:30px;
}

nav a{
color:white;
text-decoration:none;
font-weight:500;
transition:0.3s;
}

nav a:hover{
color:#e6c7a3;
}

/* HERO */

.hero{
height:100vh;
background:url("https://images.unsplash.com/photo-1495474472287-4d71bcdd2085") center/cover no-repeat;
display:flex;
align-items:center;
justify-content:center;
text-align:center;
color:white;
position:relative;
}

.hero::after{
content:"";
position:absolute;
width:100%;
height:100%;
background:rgba(0,0,0,0.45);
top:0;
left:0;
}

.hero-content{
position:relative;
z-index:1;
animation:fadeUp 1.5s ease;
}

.hero h1{
font-size:55px;
margin-bottom:10px;
}

.hero p{
font-size:18px;
margin-bottom:20px;
}

.hero button{
padding:12px 25px;
border:none;
background:#c8a27c;
color:white;
font-size:16px;
border-radius:30px;
cursor:pointer;
transition:0.3s;
}

.hero button:hover{
background:#a57b5a;
}

/* MENU */

section{
padding:80px 8%;
}

.title{
text-align:center;
font-size:32px;
margin-bottom:40px;
}

.menu{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:25px;
}

.card{
background:white;
border-radius:12px;
overflow:hidden;
box-shadow:0 8px 20px rgba(0,0,0,0.08);
transition:0.4s;
}

.card:hover{
transform:translateY(-10px) scale(1.02);
}

.card img{
width:100%;
height:200px;
object-fit:cover;
}

.card h3{
padding:15px;
}

.card p{
padding:0 15px 20px;
font-size:14px;
color:#666;
}

/* ABOUT */

.about{
display:grid;
grid-template-columns:1fr 1fr;
gap:40px;
align-items:center;
}

.about img{
width:100%;
border-radius:12px;
}

/* FOOTER */

footer{
background:#5c3a2e;
color:white;
text-align:center;
padding:25px;
}

/* ANIMATION */

@keyframes fadeUp{
from{
opacity:0;
transform:translateY(40px);
}
to{
opacity:1;
transform:translateY(0);
}
}

/* RESPONSIVE */

@media(max-width:768px){

.hero h1{
font-size:36px;
}

.about{
grid-template-columns:1fr;
}

nav ul{
display:none;
}

}

</style>
</head>

<body>

<nav>
<div class="logo">☕ CozyCup</div>
<ul>
<li><a href="#">Home</a></li>
<li><a href="#menu">Menu</a></li>
<li><a href="#about">About</a></li>
<li><a href="#">Contact</a></li>
</ul>
</nav>

<section class="hero">

<div class="hero-content">
<h1>Fresh Coffee Everyday</h1>
<p>Warm, cozy, and handcrafted coffee just for you</p>
<button>View Menu</button>
</div>

</section>

<section id="menu">

<h2 class="title">Our Coffee</h2>

<div class="menu">

<div class="card">
<img src="https://images.unsplash.com/photo-1511920170033-f8396924c348">
<h3>Espresso</h3>
<p>Strong and rich espresso made from premium beans.</p>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1509042239860-f550ce710b93">
<h3>Cappuccino</h3>
<p>Classic cappuccino with smooth milk foam.</p>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1507133750040-4a8f57021571">
<h3>Latte</h3>
<p>Creamy latte with silky steamed milk.</p>
</div>

</div>

</section>

<section id="about">

<h2 class="title">About Our Café</h2>

<div class="about">

<div>
<p>
At CozyCup Coffee we believe coffee is more than a drink —
it's an experience. Our café combines warm interior design,
comfortable seating, and expertly brewed coffee to create
a welcoming place for everyone.
</p>
<br>
<p>
Whether you're working, relaxing, or meeting friends,
CozyCup is your perfect coffee destination.
</p>
</div>

<img src="https://images.unsplash.com/photo-1442512595331-e89e73853f31">

</div>

</section>

<footer>
<p>© 2026 CozyCup Coffee | Made with ☕</p>
</footer>

</body>
</html>
```
