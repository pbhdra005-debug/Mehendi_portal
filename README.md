<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>JOYITA MEHENDI ARTIST</title>

<!-- GOOGLE FONT -->

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins',sans-serif;
    scroll-behavior:smooth;
}

body{
    background:#fffaf5;
    overflow-x:hidden;
}


header{

    width:100%;
    padding:20px 8%;
    background:linear-gradient(135deg,#8b4513,#c96f2d);
    display:flex;
    justify-content:space-between;
    align-items:center;
    position:sticky;
    top:0;
    z-index:1000;
    animation:slideDown 1s ease;
}

header h1{
    color:white;
    font-size:38px;
    font-weight:700;
    letter-spacing:1px;
}

nav a{

    color:white;
    text-decoration:none;
    margin-left:30px;
    font-size:18px;
    font-weight:500;
    transition:.4s;
    position:relative;
}

nav a:hover{
    color:#f8c89f;
}

nav a::after{

    content:'';
    position:absolute;
    width:0%;
    height:3px;
    background:white;
    left:0;
    bottom:-6px;
    transition:.4s;
}

nav a:hover::after{
    width:100%;
}


.hero{

    min-height:100vh;
    background-image:linear-gradient(rgba(0,0,0,0.55), rgba(0,0,0,0.55)), url('m30 (79).jpeg');
    background-size:cover;
    background-position:center;
    background-repeat:no-repeat;
    display:flex;
    justify-content:center;
    align-items:center;
    padding:60px 8%;
}

.hero-container{

    width:100%;
    display:flex;
    justify-content:space-between;
    align-items:center;
    gap:100px;
}


.hero-images{

    justify-content: center;
    display:flex;
    gap:25px;
    animation:fadeLeft 1.5s ease;
}

.hero-images img{

    width:400px;
    height:500px;
    object-fit:cover;
    border-radius:20px;
    box-shadow:0 10px 30px rgba(0,0,0,0.4);
    transition:.5s;
}

.hero-images img:hover{
    transform:scale(1.05) rotate(2deg);
}


.hero-content{

    max-width:500px;
    color:white;
    animation:fadeRight 1.5s ease;
}

.hero-content h2{

    font-size:65px;
    line-height:1.2;
    margin-bottom:20px;
}

.hero-content p{

    font-size:22px;
    margin-bottom:35px;
    color:#f1f1f1;
}

.btn{

    display:inline-block;
    padding:15px 35px;
    background:#ffb37b;
    color:#5c2d0c;
    text-decoration:none;
    border-radius:50px;
    font-size:18px;
    font-weight:600;
    transition:.4s;
}

.btn:hover{

    background:white;
    transform:translateY(-5px);
}


.services-section{
    padding:100px 8%;
}

.section-title{

    text-align:center;
    margin-bottom:60px;
    animation:fadeUp 1s ease;
}

.section-title h2{

    font-size:45px;
    color:#8b4513;
}

.services{

    display:grid;
    grid-template-columns:
    repeat(auto-fit,minmax(250px,1fr));
    gap:30px;
}

.service-box{

    background:white;
    padding:40px 30px;
    border-radius:25px;
    text-align:center;
    box-shadow:0 8px 20px rgba(0,0,0,0.08);
    transition:.5s;
}

.service-box:hover{
    transform:translateY(-12px);
}

.service-box h3{

    color:#8b4513;
    font-size:25px;
    margin-bottom:15px;
}

.service-box p{
    color:#666;
}


.gallery-section{
    padding:100px 8%;
}

.gallery{

    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
    gap:25px;
}

.gallery img{

    width:100%;
    height:420px;
    object-fit:cover;
    border-radius:25px;
    transition:.5s;
}

.gallery img:hover{
    transform:scale(1.08);
}


.pricing-section{
    padding:100px 8%;
}

.pricing{

    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(320px,1fr));
    gap:30px;
}

.price-card{

    background:white;
    padding:40px;
    border-radius:25px;
    box-shadow:0 8px 20px rgba(0,0,0,0.08);
    transition:.5s;
    max-height:550px;
    overflow-y:auto;
}

.price-card:hover{
    transform:translateY(-10px);
}

.price-card h1{

    color:#8b4513;
    font-size:28px;
    margin-bottom:25px;
}

.price-card h3{

    color:#444;
    line-height:2;
    font-size:17px;
    font-weight:500;
}


.contact-section{
    padding:100px 8%;
}

.contact-form{

    max-width:700px;
    margin:auto;
    background:white;
    padding:50px;
    border-radius:30px;
    box-shadow:0 8px 20px rgba(0,0,0,0.08);
    animation:fadeUp 1.2s ease;
}

.contact-form input,
.contact-form textarea{

    width:100%;
    padding:18px;
    margin-bottom:20px;
    border:1px solid #ddd;
    border-radius:15px;
    font-size:16px;
    outline:none;
}

.contact-form button{

    width:100%;
    padding:18px;
    border:none;
    background:#8b4513;
    color:white;
    border-radius:15px;
    font-size:18px;
    cursor:pointer;
    transition:.4s;
}

.contact-form button:hover{
    background:#c96f2d;
}


footer{

    background:#5c2d0c;
    color:white;
    text-align:center;
    padding:30px;
    margin-top:50px;
}

.whatsapp{

    position:fixed;
    right:25px;
    bottom:25px;
    width:65px;
    height:65px;
    background:#25d366;
    border-radius:50%;
    display:flex;
    justify-content:center;
    align-items:center;
    color:white;
    font-size:30px;
    text-decoration:none;
    box-shadow:0 5px 15px rgba(0,0,0,0.3);
    animation:float 2s infinite;
}


@keyframes slideDown{

    from{
        transform:translateY(-100px);
        opacity:0;
    }

    to{
        transform:translateY(0);
        opacity:1;
    }
}

@keyframes fadeLeft{

    from{
        transform:translateX(-100px);
        opacity:0;
    }

    to{
        transform:translateX(0);
        opacity:1;
    }
}

@keyframes fadeRight{

    from{
        transform:translateX(100px);
        opacity:0;
    }

    to{
        transform:translateX(0);
        opacity:1;
    }
}

@keyframes fadeUp{

    from{
        transform:translateY(80px);
        opacity:0;
    }

    to{
        transform:translateY(0);
        opacity:1;
    }
}

@keyframes float{

    0%{
        transform:translateY(0px);
    }

    50%{
        transform:translateY(-10px);
    }

    100%{
        transform:translateY(0px);
    }
}

@media(max-width:992px){

.hero-container{
    flex-direction:column;
    text-align:center;
}

.hero-images{
    flex-direction:column;
}

.hero-images img{
    width:100%;
    max-width:400px;
    height:auto;
}

.hero-content h2{
    font-size:42px;
}

nav{
    display:none;
}

}

@media(max-width:600px){

header h1{
    font-size:28px;
}

.hero-content h2{
    font-size:34px;
}

.section-title h2{
    font-size:34px;
}

}

</style>
</head>

<body>

<header>

<h1>JOYITA MEHENDI ARTIST</h1>

<nav>

<a href="#home">Home</a>
<a href="#services">Services</a>
<a href="#gallery">Gallery</a>
<a href="#pricing">Pricing</a>
<a href="#contact">Contact</a>

</nav>

</header>


<section class="hero" id="home">

<div class="hero-container">

<div class="hero-images">

<img src="m30 (48).jpeg" alt="">
<img src="m30 (30).jpeg" alt="">

</div>

<div class="hero-content">

<h2>
Beautiful Mehendi For Every Occasion
</h2>

<p>
Bridal • Arabic • Royal • Festival Mehendi Designs
</p>

<a href="#contact" class="btn">
Book Now
</a>

</div>

</div>

</section>


<section class="services-section" id="services">

<div class="section-title">
<h2>Our Services</h2>
</div>

<div class="services">

<div class="service-box">

<h3>Bridal Mehendi</h3>

<p>
Elegant and detailed bridal mehendi designs for weddings.
</p>

</div>

<div class="service-box">

<h3>Arabic Mehendi</h3>

<p>
Modern Arabic patterns with stylish finishing.
</p>

</div>

<div class="service-box">

<h3>Festival Mehendi</h3>

<p>
Special mehendi designs for Eid, Diwali, Baby Shower and celebrations.
</p>

</div>

<div class="service-box">

<h3>Party Mehendi</h3>

<p>
Quick and trendy designs for parties and events.
</p>

</div>
<div class="service-box">

<h3> Mehendi Classes With Certification</h3>

<p>
JOYITA MEHENDI CLASSES -----
🌱 REGISTRATION AMOUNT=2500/- <br>
**Advance payment 2500/is not refundable,so if you are confirm about your participation then only book your seat** <br>
🌱 Contact 8296835001 For More Info <br>
</p>

</div>

</div>

</section>


<section class="gallery-section" id="gallery">

<div class="section-title">
<h2>Gallery</h2>
</div>

<div class="gallery">

<img src="m30 (79).jpeg" alt="">
<img src="m30 (12).jpeg" alt="">
<img src="m30 (30).jpeg" alt="">
<img src="m30 (2).jpeg" alt="">
<img src="m30 (15).jpeg" alt="">
<img src="m30 (8).jpeg" alt="">
<img src="m30 (74).jpeg" alt="">
<img src="m30 (25).jpeg" alt="">
<img src="m30 (37).jpeg" alt="">
<img src="m30 (45).jpeg" alt="">
<img src="m30 (78).jpeg" alt="">
<img src="m30 (64).jpeg" alt="">

</div>

</section>

<section class="pricing-section" id="pricing">

<div class="section-title">
<h2>Pricing</h2>
</div>

<div class="pricing">

<div class="price-card">

<h1>BRIDAL MEHENDI PACKAGE</h1>

<h3>

🌱 Bridal starting without figures and wedding elements
(length upto either elbow or 4 fingers above elbow,
ankle or 4 fingers above ankle)= 3500/- <br><br>

🌱 With wedding elements + 2 figures = 4500/- <br><br>

🌱 With wedding elements + 4 figures = 5500/- <br><br>

🌱 Extra length = 300/- each <br><br>

🌱 Extra figure = 300/- per figure <br><br>

🌱 Advance compulsory (not refundable) <br><br>

🌱 Conveyance extra

</h3>

</div>

<div class="price-card">

<h1>BABY SHOWER & ENGAGEMENT PACKAGE</h1>

<h3>

🌱 Starting rate = 1500/- without figures <br><br>

🌱 Elbow length = 3000/- (with 2 figures) <br><br>

🌱 Extra figure = 200/- <br><br>

🌱 Extra length = 300/- per 3 fingers <br><br>

🌱 Feet = 300/- starting <br><br>

🌱 Advance compulsory (not refundable) <br><br>

🌱 Conveyance extra

</h3>

</div>

<div class="price-card">

<h1>WITHOUT PACKAGE</h1>

<h3>

🌱 Upto elbow = 1500/- <br><br>

🌱 Semi bridal length = 1000/- <br><br>

🌱 Wrist length = 700/-

</h3>

</div>

</div>

</section>


<section class="contact-section" id="contact">

<div class="section-title">
<h2>Contact Us</h2>
</div>

<div class="contact-form">
<form action="https://formsubmit.co/aninditabose8119@gmail.com" method="POST">
<form action="https://forsubmit.co/wa.me/918296835001" class="whatsapp">


<input
type="text"
name="Name"
placeholder="Your Name"
required>

<input
type="email"
name="Email"
placeholder="Your Email"
required>

<input
type="tel"
name="Phone"
placeholder="Phone Number"
required>

<textarea
name="Message"
rows="5"
placeholder="Your Message"
required></textarea>

<!-- Hidden Settings -->

<input
type="hidden"
name="_subject"
value="New Booking Request - JOYITA MEHENDI ARTIST">

<input
type="hidden"
name="_captcha"
value="false">

<input
type="hidden"
name="_template"
value="table">

<button type="submit">
Send Booking Request
</button>

</form>
</div>

</section>


<footer>

<p>
 JOYITA MEHENDI ARTIST | All Rights Reserved
</p>

</footer>




</body>
</html>
