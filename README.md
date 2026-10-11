# Galabant
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Galabant – T-shirts for Men & Women</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
:root{--red:#f43f5e;--dark:#2d2d2d;--muted:#8a8a8a;--grey:#ececec;--border:#e4e4e4}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{font-family:"Poppins",system-ui,sans-serif;color:#1c1c1c;background:#fff;line-height:1.5}
a{color:inherit;text-decoration:none}
.container{width:min(1100px,92%);margin-inline:auto}
.center{text-align:center;margin-top:28px}
.muted{color:var(--muted);font-size:12px}
.btn{display:inline-block;background:var(--red);color:#fff;padding:10px 22px;border-radius:4px;font-size:12px;font-weight:600;border:0;cursor:pointer}
.btn.small{padding:7px 18px;font-size:11px}
.btn-outline{display:inline-block;border:1px solid var(--red);color:var(--red);padding:5px 16px;border-radius:4px;font-size:11px;font-weight:500}
.topbar{background:var(--dark);color:#fff;font-size:10px;padding:8px 0}
.topbar .container{display:flex;justify-content:space-between}
.header{background:#fff;border-bottom:1px solid var(--border);position:sticky;top:0;z-index:10}
.header .container{display:flex;align-items:center;justify-content:space-between;gap:20px;padding:14px 0;flex-wrap:wrap}
.logo{font-weight:800;font-size:24px;color:var(--red);letter-spacing:1px}
.logo.light{color:#fff}
.nav{display:flex;gap:22px;font-size:12px;font-weight:500}
.nav a.active,.nav a:hover{color:var(--red)}
.header-tools{display:flex;align-items:center;gap:14px;font-size:12px}
.header-tools input{border:1px solid var(--border);border-radius:20px;padding:6px 14px;font:inherit;font-size:11px;width:130px}
.hero{background:var(--grey)}
.hero-inner{display:flex;align-items:center;justify-content:space-between;min-height:340px;gap:30px}
.hero-text{max-width:380px;padding:30px 0}
.offer{font-size:18px}
.offer span,.hero h1 span{color:var(--red)}
.hero h1{font-size:30px;font-weight:800;line-height:1.25;margin:6px 0 14px}
.hero .btn{margin-top:18px}
.hero-img{flex:1;max-width:420px;align-self:flex-end}
.hero-img .ph{height:320px;border-radius:8px 8px 0 0}
.ph{background:#cfcfcf;display:grid;place-items:center;color:rgba(0,0,0,.35);font-size:12px;width:100%}
.section{padding:56px 0}
.section.grey{background:var(--grey)}
.section h2{text-align:center;font-size:18px;font-weight:700;text-transform:uppercase;margin-bottom:28px}
.grid-4{display:grid;grid-template-columns:repeat(4,1fr);gap:18px}
.grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
.cat{position:relative;display:block;border-radius:6px;overflow:hidden}
.categories .ph{height:210px}
.occasions{max-width:640px;margin:36px auto 0}
.occasions .ph{height:150px}
.cat span{position:absolute;left:0;right:0;bottom:0;background:rgba(255,255,255,.88);text-align:center;font-size:11px;font-weight:600;padding:4px 0;text-transform:uppercase}
.cat span.on{background:var(--red);color:#fff}
.card{background:#fff;border:1px solid var(--border);border-radius:8px;padding:14px;text-align:center}
.card.active{border-color:var(--red);box-shadow:0 0 0 1px var(--red)}
.thumb{height:120px;border-radius:6px;margin-bottom:10px}
.desc{font-size:10px;color:var(--muted);margin-bottom:6px}
.stars{color:#f5b301;font-size:11px;letter-spacing:1px}
.price{font-weight:700;font-size:17px;color:#555;margin:4px 0 10px}
.sale{background:var(--grey)}
.sale-inner{display:flex;align-items:center;justify-content:space-between;gap:30px;padding:24px 0}
.sale-img{max-width:420px;height:240px;border-radius:8px}
.sale-text p{font-size:18px}
.sale-text h2{font-size:24px;font-weight:800;text-align:left;text-transform:none;line-height:1.3;margin:4px 0 14px}
.sale-text h2 span{color:var(--red)}
.quote{background:#fff;border-radius:6px;padding:18px}
.qmark{color:var(--red);font-size:44px;line-height:.6;font-weight:800;display:block;margin-bottom:8px}
.quote p{font-size:9px;letter-spacing:.5px;text-transform:uppercase;color:#999;margin-bottom:14px}
.quote footer{display:flex;align-items:center;gap:8px;font-size:9px;flex-wrap:wrap}
.avatar{width:22px;height:22px;border-radius:50%;background:#bbb}
.feature{text-align:center}
.icon{display:inline-grid;place-items:center;width:48px;height:48px;border-radius:50%;background:var(--red);color:#fff;font-size:20px;margin-bottom:8px}
.feature h3{font-size:11px;text-transform:uppercase;color:var(--red)}
.feature p{font-size:9px;color:var(--muted)}
.footer{background:var(--dark);color:#fff;padding:36px 0 14px}
.footer-grid{display:grid;grid-template-columns:1.2fr 1.4fr 1fr 1fr 1.4fr;gap:24px;font-size:11px}
.footer h4{font-size:12px;margin-bottom:10px}
.footer-grid a{display:block;color:#cfcfcf;margin-bottom:4px}
.footer-grid p{color:#cfcfcf;margin-bottom:6px}
.newsletter{display:flex}
.newsletter input{flex:1;min-width:0;padding:7px 10px;border:0;border-radius:3px 0 0 3px;font:inherit;font-size:11px}
.newsletter button{background:var(--red);color:#fff;border:0;padding:0 14px;border-radius:0 3px 3px 0}
.footer-bottom{display:flex;justify-content:space-between;gap:10px;flex-wrap:wrap;font-size:9px;color:#999;margin-top:30px}
@media(max-width:900px){.grid-4{grid-template-columns:repeat(2,1fr)}.footer-grid{grid-template-columns:repeat(2,1fr)}.nav{order:3;width:100%;overflow-x:auto}}
@media(max-width:640px){.hero-inner,.sale-inner{flex-direction:column;text-align:center}.hero-img,.sale-img{max-width:100%}.grid-3{grid-template-columns:1fr}.sale-text h2{text-align:center}.topbar .container{flex-direction:column;text-align:center}}
</style>
</head>
<body>

<div class="topbar"><div class="container"><span>Welcome to Galabant</span><span>Need help? www.galabant.com</span></div></div>

<header class="header"><div class="container">
<a href="#" class="logo">GALABANT</a>
<nav class="nav">
<a href="#home" class="active">Home</a><a href="#categories">Categories</a><a href="#latest">Product</a><a href="#footer">About</a><a href="#popular">Popular Product</a><a href="#testimonial">Testimonial</a>
</nav>
<div class="header-tools"><input type="search" placeholder="Search"><a href="#">Sign Up</a><a href="#">Cart</a></div>
</div></header>

<section class="hero" id="home"><div class="container hero-inner">
<div class="hero-text">
<p class="offer">Special <span>Offer</span></p>
<h1>T-SHIRTS FOR<br>MEN &amp; <span>WOMEN</span></h1>
<p class="muted">Lorem ipsum dolor sit amet, consectetur adipiscing elit sed do eiusmod tempor.</p>
<a href="#" class="btn">Shop Now</a>
</div>
<div class="hero-img"><div class="ph">Hero image</div></div>
</div></section>

<section class="section" id="categories"><div class="container">
<h2>Product Categories</h2>
<div class="grid-4 categories">
<a href="#" class="cat"><div class="ph" style="background:#c8283c"></div><span>Women</span></a>
<a href="#" class="cat"><div class="ph" style="background:#e6a32e"></div><span>Men</span></a>
<a href="#" class="cat"><div class="ph" style="background:#cfcfcf"></div><span>Tank Top</span></a>
<a href="#" class="cat"><div class="ph" style="background:#8a8a8a"></div><span>Hoodies</span></a>
</div>
<div class="center"><a href="#" class="btn small">Shop Now</a></div>
</div></section>

<section class="section" id="latest"><div class="container">
<h2>Latest Product</h2>
<div class="grid-4">
<article class="card"><div class="thumb" style="background:#111"></div><p class="desc">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed</p><div class="stars">★★★★★</div><p class="price">$11.25</p><a href="#" class="btn-outline">Shop Now</a></article>
<article class="card active"><div class="thumb" style="background:#1d1d1d"></div><p class="desc">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed</p><div class="stars">★★★★★</div><p class="price">$25.00</p><a href="#" class="btn small">Shop Now</a></article>
<article class="card"><div class="thumb" style="background:#d9304a"></div><p class="desc">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed</p><div class="stars">★★★★★</div><p class="price">$10.25</p><a href="#" class="btn-outline">Shop Now</a></article>
<article class="card"><div class="thumb" style="background:#f2f2f2"></div><p class="desc">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed</p><div class="stars">★★★★★</div><p class="price">$05.25</p><a href="#" class="btn-outline">Shop Now</a></article>
</div>
<div class="center"><a href="#" class="btn small">View All</a></div>
</div></section>

<section class="sale"><div class="container sale-inner">
<div class="ph sale-img">Banner image</div>
<div class="sale-text">
<p>Special Offer</p>
<h2>WEEKENDS <span>SALE</span><br>UPTO <span>50% OFF</span></h2>
<a href="#" class="btn small">Shop Now</a>
</div>
</div></section>

<section class="section" id="popular"><div class="container">
<h2>Popular Product</h2>
<div class="grid-4">
<article class="card"><div class="thumb" style="background:#111"></div><p class="desc">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed</p><div class="stars">★★★★★</div><p class="price">$11.25</p><a href="#" class="btn-outline">Shop Now</a></article>
<article class="card active"><div class="thumb" style="background:#1d1d1d"></div><p class="desc">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed</p><div class="stars">★★★★★</div><p class="price">$25.00</p><a href="#" class="btn small">Shop Now</a></article>
<article class="card"><div class="thumb" style="background:#d9304a"></div><p class="desc">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed</p><div class="stars">★★★★★</div><p class="price">$10.25</p><a href="#" class="btn-outline">Shop Now</a></article>
<article class="card"><div class="thumb" style="background:#f2f2f2"></div><p class="desc">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed</p><div class="stars">★★★★★</div><p class="price">$05.25</p><a href="#" class="btn-outline">Shop Now</a></article>
</div>
<div class="center"><a href="#" class="btn small">View All</a></div>
<div class="grid-3 occasions">
<a href="#" class="cat"><div class="ph" style="background:#7a5a52"></div><span>Christmas</span></a>
<a href="#" class="cat"><div class="ph" style="background:#2a3446"></div><span class="on">Events</span></a>
<a href="#" class="cat"><div class="ph" style="background:#a86a52"></div><span>Fun</span></a>
</div>
</div></section>

<section class="section grey" id="testimonial"><div class="container">
<h2>Customer Testimonial</h2>
<div class="grid-3">
<blockquote class="quote"><span class="qmark">&ldquo;</span><p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore.</p><footer><span class="avatar"></span><b>Robert Brennan</b><span class="stars">★★★★★</span></footer></blockquote>
<blockquote class="quote"><span class="qmark">&ldquo;</span><p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore.</p><footer><span class="avatar"></span><b>Ruth A. Rosa</b><span class="stars">★★★★★</span></footer></blockquote>
<blockquote class="quote"><span class="qmark">&ldquo;</span><p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore.</p><footer><span class="avatar"></span><b>Carol A. Rivas</b><span class="stars">★★★★★</span></footer></blockquote>
</div>
<div class="center"><a href="#" class="btn small">View All</a></div>
</div></section>

<section class="section"><div class="container grid-3">
<div class="feature"><span class="icon">🚚</span><h3>Free Shipping</h3><p>Lorem ipsum dolor sit amet, sed do eiusmod.</p></div>
<div class="feature"><span class="icon">◎</span><h3>Money Back</h3><p>Lorem ipsum dolor sit amet, sed do eiusmod.</p></div>
<div class="feature"><span class="icon">🔒</span><h3>Secure Payment</h3><p>Lorem ipsum dolor sit amet, sed do eiusmod.</p></div>
</div></section>

<footer class="footer" id="footer">
<div class="container footer-grid">
<div><a href="#" class="logo light">GALABANT</a></div>
<div><h4>Contact Us</h4><p>+1 41 456 981 659</p><p>Street No. 04, New York, USA</p><p>info@galabant.com</p></div>
<div><h4>Useful Link</h4><a href="#">Home</a><a href="#">About Us</a><a href="#">Product</a><a href="#">Contact</a></div>
<div><h4>Categories</h4><a href="#">T-Shirt</a><a href="#">Tank Top</a><a href="#">Hoodies</a><a href="#">Sweater</a></div>
<div><h4>Newsletter Subscribe</h4><form class="newsletter" onsubmit="return false"><input type="email" placeholder="Email"><button type="submit">Go</button></form></div>
</div>
<div class="container footer-bottom"><span>Terms and Conditions · Privacy Policy</span><span>Copyright by Galabant 2026</span><span>VISA · Mastercard · PayPal</span></div>
</footer>

</body>
</html>