<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Babu Fast Food</title>

<style>
body{
  margin:0;
  font-family:"Times New Roman", serif;
  background:#f4f4f4;
}

/* SPLASH SCREEN */
#splash{
  position:fixed;
  inset:0;
  background:#111;
  color:#fff;
  display:flex;
  align-items:center;
  justify-content:center;
  z-index:9999;
}
.splash-box{
  text-align:center;
}
.splash-box img{
  width:160px;
  height:160px;
}
.splash-box h1{
  margin:15px 0 5px;
  font-size:32px;
  color:#ff3d00;
}
.splash-box p{
  font-size:16px;
}

/* HEADER */
header{
  background:#ff3d00;
  color:#fff;
  padding:15px;
  display:flex;
  justify-content:space-between;
  align-items:center;
  flex-wrap:wrap;
}
.logo{
  display:flex;
  align-items:center;
}
.logo img{
  width:48px;
  height:48px;
  margin-right:10px;
}
nav a{
  color:#fff;
  margin-left:12px;
  text-decoration:none;
  font-weight:bold;
}

/* HERO */
.hero{
  background:#000;
  color:#fff;
  padding:50px 20px;
  text-align:center;
}

/* SECTIONS */
.menu,.order,.location{
  padding:20px;
}
.menu h2,.order h2,.location h2{
  text-align:center;
}

/* ITEMS */
.item{
  background:#fff;
  padding:15px;
  margin-bottom:20px;
  border-radius:10px;
}
.item img{
  width:100%;
  max-height:200px;
  object-fit:cover;
  border-radius:10px;
}
button{
  background:#ff3d00;
  color:#fff;
  border:none;
  padding:10px 15px;
  border-radius:5px;
  cursor:pointer;
  margin-top:10px;
}
input,textarea{
  width:100%;
  padding:10px;
  margin:8px 0;
}

/* FOOTER */
footer{
  background:#222;
  color:#fff;
  text-align:center;
  padding:10px;
}

/* WHATSAPP */
.whatsapp-float{
  position:fixed;
  bottom:20px;
  right:20px;
  background:#25D366;
  color:#fff;
  padding:12px 18px;
  border-radius:50px;
  text-decoration:none;
  font-weight:bold;
}

/* MAP */
.map-box{
  width:100%;
  height:300px;
  border:0;
  border-radius:10px;
}
</style>
</head>

<body>

<!-- SPLASH LOGO -->
<div id="splash">
  <div class="splash-box">
    <!-- CHEF SHAPE ICON -->
    <img src="https://cdn-icons-png.flaticon.com/512/1046/1046784.png" alt="Chef Logo">
    <h1>Babu Fast Food</h1>
    <p>Classic Taste & Fine Quality</p>
    <p>Phone: 0112027146</p>
  </div>
</div>

<header>
  <div class="logo">
    <img src="https://cdn-icons-png.flaticon.com/512/1046/1046784.png">
    <h2>Babu Fast Food</h2>
  </div>
  <nav>
    <a href="#menu">Menu</a>
    <a href="#order">Order</a>
    <a href="#location">Location</a>
  </nav>
</header>

<section class="hero">
  <h1>Welcome to Babu Fast Food</h1>
  <p>Serving Honest Food Since Day One</p>
  <p>Call Us: 0112027146</p>
</section>

<section id="menu" class="menu">
<h2>Our Menu</h2>

<div class="item">
<img src="https://images.unsplash.com/photo-1550547660-d9450f859349">
<h3>Zinger Burger</h3>
<p>Price: Rs 450</p>
<button onclick="addToCart('Zinger Burger',450)">Add to Order</button>
</div>

<div class="item">
<img src="https://images.unsplash.com/photo-1568901346375-23c9450c58cd">
<h3>Chicken Burger</h3>
<p>Price: Rs 350</p>
<button onclick="addToCart('Chicken Burger',350)">Add to Order</button>
</div>

<div class="item">
<img src="https://images.unsplash.com/photo-1604908554026-8f13a5f7b37d">
<h3>Chicken Roll</h3>
<p>Price: Rs 250</p>
<button onclick="addToCart('Chicken Roll',250)">Add to Order</button>
</div>

<div class="item">
<img src="https://images.unsplash.com/photo-1541592106381-b31e9677c0e5">
<h3>French Fries</h3>
<p>Price: Rs 200</p>
<button onclick="addToCart('French Fries',200)">Add to Order</button>
</div>
</section>

<section id="order" class="order">
<h2>Your Order</h2>
<ul id="cart"></ul>
<p id="total">Total: Rs 0</p>
<button onclick="sendWhatsApp()">Order via WhatsApp</button>
</section>

<section id="location" class="location">
<h2>Our Location</h2>
<p style="text-align:center;font-weight:bold">
Gulshan Secunderabad, Maari, Karachi
</p>
<iframe class="map-box"
src="https://www.google.com/maps?q=Gulshan+Secunderabad+Karachi&output=embed">
</iframe>
</section>

<footer>
<p>© 2026 Babu Fast Food | Phone: 0112027146</p>
</footer>

<a class="whatsapp-float"
href="https://wa.me/920112027146"
target="_blank">WhatsApp Order</a>

<script>
/* Splash hide */
setTimeout(()=>{
  document.getElementById("splash").style.display="none";
},2500);

let total=0, items=[];
function addToCart(n,p){
  items.push(n+" - Rs "+p);
  total+=p;
  document.getElementById("cart").innerHTML=
    items.map(i=>"<li>"+i+"</li>").join("");
  document.getElementById("total").innerText="Total: Rs "+total;
}
function sendWhatsApp(){
  let msg="Babu Fast Food Order%0A"+items.join("%0A")+"%0ATotal: Rs "+total;
  window.open("https://wa.me/920112027146?text="+msg,"_blank");
}
</script>

</body>
</html>
