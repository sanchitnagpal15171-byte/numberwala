<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>VIP Car Numbers</title>

<style>

body{
font-family:Arial;
margin:0;
background:#f4f4f4;
}

header{
background:#000;
color:white;
padding:15px;
text-align:center;
}

.search-box{
text-align:center;
padding:30px;
}

.search-box input{
padding:10px;
width:250px;
font-size:16px;
}

.search-box button{
padding:10px 20px;
background:#d32f2f;
color:white;
border:none;
cursor:pointer;
}

.container{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
gap:20px;
padding:30px;
}

.card{
background:white;
padding:20px;
border-radius:10px;
text-align:center;
box-shadow:0 4px 8px rgba(0,0,0,0.1);
}

.card h2{
color:#d32f2f;
font-size:28px;
}

.btn{
display:inline-block;
margin-top:10px;
padding:8px 15px;
background:black;
color:white;
text-decoration:none;
border-radius:5px;
}

.buy{
background:#28a745;
}

footer{
background:black;
color:white;
text-align:center;
padding:20px;
}

</style>

<script>

function searchNumber() {

let input = document.getElementById("search").value.toUpperCase();
let cards = document.getElementsByClassName("card");

for (let i = 0; i < cards.length; i++) {

let number = cards[i].getElementsByTagName("h2")[0];

if (number.innerHTML.indexOf(input) > -1) {
cards[i].style.display = "";
} else {
cards[i].style.display = "none";
}

}

}

</script>

</head>

<body>

<header>
<h1>VIP Car Numbers</h1>
<p>Buy Premium Fancy Number Plates</p>
</header>

<div class="search-box">

<input type="text" id="search" placeholder="Search VIP Number">
<button onclick="searchNumber()">Search</button>

</div>

<div class="container">

<div class="card">
<h2>0001</h2>
<p>Super VIP Number</p>
<a class="btn buy" href="mailto:vipnumbers@gmail.com?subject=Booking for VIP Number 0001">Buy / Book</a>
</div>

<div class="card">
<h2>0786</h2>
<p>Lucky Number</p>
<a class="btn buy" href="mailto:vipnumbers@gmail.com?subject=Booking for VIP Number 0786">Buy / Book</a>
</div>

<div class="card">
<h2>9999</h2>
<p>Premium VIP Number</p>
<a class="btn buy" href="mailto:vipnumbers@gmail.com?subject=Booking for VIP Number 9999">Buy / Book</a>
</div>

<div class="card">
<h2>1111</h2>
<p>Luxury VIP Number</p>
<a class="btn buy" href="mailto:vipnumbers@gmail.com?subject=Booking for VIP Number 1111">Buy / Book</a>
</div>

<div class="card">
<h2>4444</h2>
<p>Premium Number</p>
<a class="btn buy" href="mailto:vipnumbers@gmail.com?subject=Booking for VIP Number 4444">Buy / Book</a>
</div>

<div class="card">
<h2>5555</h2>
<p>Fancy VIP Number</p>
<a class="btn buy" href="mailto:vipnumbers@gmail.com?subject=Booking for VIP Number 5555">Buy / Book</a>
</div>

</div>

<footer>

<p>Contact Us</p>

<a class="btn" href="tel:+919999999999">📞 Call</a>
<a class="btn" href="https://wa.me/919999999999">💬 WhatsApp</a>
<a class="btn" href="mailto:vipnumbers@gmail.com">📧 Email</a>

</footer>

</body>
</html>
