<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Sachin Web Solutions | Professional Web Development</title>

<meta name="description" content="Sachin Web Solutions provides professional WordPress, Elementor, Business, E-commerce and SEO website development services.">

<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">

<style>

/* =========================
   RESET
========================= */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
}

body{
    font-family:Arial,Helvetica,sans-serif;
    background:#080b1a;
    color:#fff;
    line-height:1.6;
}

a{
    text-decoration:none;
    color:inherit;
}

.container{
    width:90%;
    max-width:1200px;
    margin:auto;
}


/* =========================
   NAVBAR
========================= */

nav{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    z-index:9999;

    background:rgba(8,11,26,.85);
    backdrop-filter:blur(15px);

    border-bottom:1px solid rgba(255,255,255,.1);
}

.nav-box{
    min-height:75px;

    display:flex;
    align-items:center;
    justify-content:space-between;
}

.logo{
    font-size:24px;
    font-weight:900;

    background:linear-gradient(
        90deg,
        #00eaff,
        #7c3cff,
        #ff3cac
    );

    -webkit-background-clip:text;
    color:transparent;
}

.menu{
    display:flex;
    gap:28px;
    align-items:center;
    list-style:none;
}

.menu a{
    color:#d9ddf0;
    font-size:15px;
    font-weight:600;
    transition:.3s;
}

.menu a:hover{
    color:#00eaff;
}

.nav-btn{
    padding:10px 20px;
    border-radius:30px;

    background:linear-gradient(
        90deg,
        #7c3cff,
        #ff3cac
    );

    color:#fff!important;
}


/* =========================
   HERO
========================= */

.hero{
    min-height:100vh;

    display:flex;
    align-items:center;

    padding-top:100px;

    position:relative;
    overflow:hidden;

    background:
    radial-gradient(
        circle at 10% 20%,
        rgba(0,234,255,.18),
        transparent 30%
    ),
    radial-gradient(
        circle at 90% 20%,
        rgba(255,60,172,.20),
        transparent 30%
    ),
    radial-gradient(
        circle at 50% 90%,
        rgba(124,60,255,.20),
        transparent 35%
    ),
    #080b1a;
}

.hero-grid{
    display:grid;
    grid-template-columns:1.15fr .85fr;
    gap:60px;
    align-items:center;
}

.badge{
    display:inline-flex;
    align-items:center;
    gap:8px;

    padding:9px 18px;

    border-radius:30px;

    background:rgba(0,234,255,.1);
    border:1px solid rgba(0,234,255,.35);

    color:#00eaff;

    font-size:14px;
    font-weight:700;

    margin-bottom:22px;
}

h1{
    font-size:clamp(43px,6vw,76px);
    line-height:1.04;

    margin-bottom:24px;
}

.gradient-text{
    background:linear-gradient(
        90deg,
        #00eaff,
        #7c3cff,
        #ff3cac,
        #ff9d00
    );

    -webkit-background-clip:text;
    color:transparent;

    background-size:300% 300%;

    animation:gradientMove 5s ease infinite;
}

@keyframes gradientMove{

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

.hero p{
    color:#b8bfd5;
    max-width:650px;
    font-size:18px;
    margin-bottom:30px;
}

.buttons{
    display:flex;
    flex-wrap:wrap;
    gap:15px;
}

.btn{
    display:inline-flex;
    align-items:center;
    justify-content:center;
    gap:9px;

    padding:14px 25px;

    border-radius:10px;

    font-weight:800;

    transition:.3s;
}

.btn-primary{
    background:linear-gradient(
        90deg,
        #00c6ff,
        #0072ff
    );

    color:#fff;

    box-shadow:
    0 10px 30px rgba(0,114,255,.3);
}

.btn-primary:hover{
    transform:translateY(-4px) scale(1.02);
}

.btn-pink{
    background:linear-gradient(
        90deg,
        #7c3cff,
        #ff3cac
    );

    color:#fff;

    box-shadow:
    0 10px 30px rgba(255,60,172,.25);
}

.btn-pink:hover{
    transform:translateY(-4px);
}


/* =========================
   HERO VISUAL
========================= */

.hero-visual{
    position:relative;
    height:470px;

    display:flex;
    align-items:center;
    justify-content:center;
}

.glow-circle{
    position:absolute;

    width:330px;
    height:330px;

    border-radius:50%;

    background:linear-gradient(
        135deg,
        #00eaff,
        #7c3cff,
        #ff3cac
    );

    filter:blur(2px);

    animation:rotateCircle 8s linear infinite;
}

@keyframes rotateCircle{

    from{
        transform:rotate(0deg);
    }

    to{
        transform:rotate(360deg);
    }

}

.web-card{
    position:relative;
    z-index:2;

    width:350px;

    padding:28px;

    border-radius:25px;

    background:rgba(13,17,40,.88);

    border:1px solid rgba(255,255,255,.2);

    backdrop-filter:blur(15px);

    box-shadow:
    0 30px 80px rgba(0,0,0,.45);

    animation:floatCard 4s ease-in-out infinite;
}

@keyframes floatCard{

    0%,100%{
        transform:translateY(0);
    }

    50%{
        transform:translateY(-15px);
    }

}

.browser{
    border-radius:15px;
    overflow:hidden;

    background:#11162d;
}

.browser-top{
    height:42px;

    display:flex;
    align-items:center;

    gap:7px;

    padding:0 14px;

    background:#191f3c;
}

.browser-dot{
    width:10px;
    height:10px;
    border-radius:50%;
}

.dot1{background:#ff4d6d;}
.dot2{background:#ffc107;}
.dot3{background:#00d084;}

.browser-content{
    padding:28px 20px;
}

.preview-title{
    height:28px;
    width:80%;

    border-radius:20px;

    background:linear-gradient(
        90deg,
        #00eaff,
        #7c3cff
    );

    margin-bottom:15px;
}

.preview-line{
    height:10px;
    width:90%;

    background:#303957;

    border-radius:20px;

    margin:10px 0;
}

.preview-line.short{
    width:60%;
}

.preview-button{
    display:inline-block;

    margin-top:15px;

    padding:10px 18px;

    border-radius:8px;

    background:linear-gradient(
        90deg,
        #ff3cac,
        #7c3cff
    );

    font-size:12px;
}


/* =========================
   SECTION
========================= */

section{
    padding:100px 0;
}

.section-title{
    text-align:center;
    max-width:750px;
    margin:0 auto 55px;
}

.section-title h2{
    font-size:43px;
    margin-bottom:12px;

    background:linear-gradient(
        90deg,
        #00eaff,
        #7c3cff,
        #ff3cac
    );

    -webkit-background-clip:text;
    color:transparent;
}

.section-title p{
    color:#9da6c0;
}


/* =========================
   ABOUT
========================= */

.about{
    background:
    linear-gradient(
        135deg,
        #0d1230,
        #120d28
    );
}

.about-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:55px;
    align-items:center;
}

.about h2{
    font-size:42px;
    margin-bottom:20px;
}

.about h2 span{
    color:#00eaff;
}

.about p{
    color:#adb5ca;
    margin-bottom:20px;
}

.about-list{
    display:grid;
    gap:12px;
}

.about-list div{
    padding:15px 18px;

    border-radius:12px;

    background:rgba(255,255,255,.05);

    border:1px solid rgba(255,255,255,.08);

    color:#e4e7f2;
}

.about-list i{
    color:#00eaff;
    margin-right:8px;
}

.about-box{
    padding:45px;

    border-radius:25px;

    background:
    linear-gradient(
        135deg,
        rgba(0,234,255,.18),
        rgba(124,60,255,.20),
        rgba(255,60,172,.15)
    );

    border:1px solid rgba(255,255,255,.12);

    box-shadow:
    0 25px 60px rgba(0,0,0,.25);
}

.about-box h3{
    font-size:30px;
    margin-bottom:15px;
}

.about-box p{
    color:#d3d7e5;
}


/* =========================
   SERVICES
========================= */

.services{
    background:#080b1a;
}

.services-grid{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:22px;
}

.service-card{
    position:relative;
    overflow:hidden;

    padding:30px 23px;

    border-radius:18px;

    background:#10152d;

    border:1px solid rgba(255,255,255,.08);

    transition:.35s;
}

.service-card::before{
    content:"";

    position:absolute;

    width:100%;
    height:4px;

    top:0;
    left:0;

    background:linear-gradient(
        90deg,
        #00eaff,
        #7c3cff,
        #ff3cac
    );
}

.service-card:hover{
    transform:translateY(-10px);

    box-shadow:
    0 20px 50px rgba(0,0,0,.35);
}

.service-icon{
    width:60px;
    height:60px;

    display:flex;
    align-items:center;
    justify-content:center;

    border-radius:16px;

    font-size:26px;

    margin-bottom:18px;

    color:#fff;
}

.blue{
    background:linear-gradient(
        135deg,
        #00c6ff,
        #0072ff
    );
}

.purple{
    background:linear-gradient(
        135deg,
        #7c3cff,
        #b02cff
    );
}

.pink{
    background:linear-gradient(
        135deg,
        #ff3cac,
        #ff5e62
    );
}

.orange{
    background:linear-gradient(
        135deg,
        #ff9d00,
        #ff4d00
    );
}

.green{
    background:linear-gradient(
        135deg,
        #00d084,
        #00a86b
    );
}

.service-card h3{
    margin-bottom:10px;
    font-size:19px;
}

.service-card p{
    color:#969fb8;
    font-size:14px;
}


/* =========================
   PRICING
========================= */

.pricing{
    background:
    linear-gradient(
        135deg,
        #0d1230,
        #170d29
    );
}

.pricing-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:25px;
}

.price-card{
    position:relative;

    padding:35px 28px;

    border-radius:22px;

    background:rgba(255,255,255,.05);

    border:1px solid rgba(255,255,255,.1);

    backdrop-filter:blur(10px);

    transition:.3s;
}

.price-card:hover{
    transform:translateY(-8px);
}

.price-card.featured{
    border:2px solid #7c3cff;

    background:
    linear-gradient(
        145deg,
        rgba(124,60,255,.18),
        rgba(255,60,172,.10)
    );

    transform:scale(1.04);
}

.price-card.featured:hover{
    transform:scale(1.04) translateY(-8px);
}

.popular{
    position:absolute;

    top:-14px;
    left:50%;

    transform:translateX(-50%);

    padding:6px 18px;

    border-radius:30px;

    background:linear-gradient(
        90deg,
        #7c3cff,
        #ff3cac
    );

    font-size:11px;
    font-weight:800;

    white-space:nowrap;
}

.price-card h3{
    font-size:23px;
    margin-bottom:12px;
}

.price{
    font-size:42px;
    font-weight:900;

    background:linear-gradient(
        90deg,
        #00eaff,
        #7c3cff,
        #ff3cac
    );

    -webkit-background-clip:text;
    color:transparent;

    margin-bottom:20px;
}

.price-card ul{
    list-style:none;
    margin-bottom:25px;
}

.price-card li{
    padding:8px 0;

    color:#c0c6d8;

    border-bottom:1px solid rgba(255,255,255,.06);
}


/* =========================
   PORTFOLIO
========================= */

.portfolio-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:25px;
}

.project{
    overflow:hidden;

    border-radius:20px;

    background:#10152d;

    border:1px solid rgba(255,255,255,.08);

    transition:.35s;
}

.project:hover{
    transform:translateY(-8px);
}

.project-img{
    height:210px;

    display:flex;
    align-items:center;
    justify-content:center;

    font-size:55px;

    color:#fff;
}

.project1{
    background:
    linear-gradient(
        135deg,
        #00c6ff,
        #0072ff,
        #7c3cff
    );
}

.project2{
    background:
    linear-gradient(
        135deg,
        #ff3cac,
        #7c3cff
    );
}

.project3{
    background:
    linear-gradient(
        135deg,
        #ff9d00,
        #ff3c5f
    );
}

.project-content{
    padding:24px;
}

.project-content h3{
    margin-bottom:7px;
}

.project-content p{
    color:#969fb8;
}


/* =========================
   WHY US
========================= */

.why{
    background:#080b1a;
}

.why-grid{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:20px;
}

.why-card{
    text-align:center;

    padding:30px 20px;

    background:#10152d;

    border-radius:18px;

    border:1px solid rgba(255,255,255,.08);
}

.why-card i{
    font-size:35px;

    background:linear-gradient(
        90deg,
        #00eaff,
        #ff3cac
    );

    -webkit-background-clip:text;
    color:transparent;
}

.why-card strong{
    display:block;
    margin-top:15px;
}

.why-card p{
    color:#969fb8;
    font-size:14px;
    margin-top:8px;
}


/* =========================
   CONTACT
========================= */

.contact{
    background:
    radial-gradient(
        circle at 20% 20%,
        rgba(0,234,255,.15),
        transparent 30%
    ),
    radial-gradient(
        circle at 80% 80%,
        rgba(255,60,172,.15),
        transparent 30%
    ),
    #0b0f22;
}

.contact-box{
    max-width:900px;

    margin:auto;

    text-align:center;

    padding:65px 30px;

    border-radius:30px;

    background:
    linear-gradient(
        135deg,
        rgba(0,234,255,.12),
        rgba(124,60,255,.15),
        rgba(255,60,172,.12)
    );

    border:1px solid rgba(255,255,255,.12);
}

.contact-box h2{
    font-size:42px;
    margin-bottom:15px;
}

.contact-box p{
    color:#adb5ca;
    margin-bottom:25px;
}

.phone{
    font-size:30px;
    font-weight:900;

    color:#00eaff;

    margin-bottom:25px;
}


/* =========================
   FOOTER
========================= */

footer{
    padding:35px 0;

    text-align:center;

    background:#050711;

    color:#7f899f;
}

footer strong{
    background:linear-gradient(
        90deg,
        #00eaff,
        #7c3cff,
        #ff3cac
    );

    -webkit-background-clip:text;
    color:transparent;
}


/* =========================
   WHATSAPP
========================= */

.whatsapp{
    position:fixed;

    right:20px;
    bottom:20px;

    width:64px;
    height:64px;

    display:flex;
    align-items:center;
    justify-content:center;

    border-radius:50%;

    background:#25D366;

    color:#fff;

    font-size:35px;

    z-index:10000;

    box-shadow:
    0 10px 35px rgba(37,211,102,.35);

    transition:.3s;
}

.whatsapp:hover{
    transform:scale(1.13);
}


/* =========================
   MOBILE
========================= */

@media(max-width:900px){

    .menu{
        display:none;
    }

    .hero-grid,
    .about-grid{
        grid-template-columns:1fr;
    }

    .services-grid,
    .why-grid{
        grid-template-columns:repeat(2,1fr);
    }

    .pricing-grid,
    .portfolio-grid{
        grid-template-columns:1fr;
    }

    .price-card.featured{
        transform:none;
    }

    .price-card.featured:hover{
        transform:translateY(-8px);
    }

    .hero-visual{
        height:400px;
    }

}


@media(max-width:600px){

    section{
        padding:75px 0;
    }

    .services-grid,
    .why-grid{
        grid-template-columns:1fr;
    }

    h1{
        font-size:43px;
    }

    .section-title h2,
    .about h2,
    .contact-box h2{
        font-size:32px;
    }

    .web-card{
        width:300px;
    }

    .glow-circle{
        width:280px;
        height:280px;
    }

    .about-box{
        padding:30px;
    }

    .phone{
        font-size:23px;
    }

    .whatsapp{
        width:58px;
        height:58px;
        right:15px;
        bottom:15px;
        font-size:31px;
    }

}

</style>
</head>


<body>


<!-- ================= NAVBAR ================= -->

<nav>

<div class="container nav-box">

<a href="#home" class="logo">
Sachin Web Solutions
</a>

<ul class="menu">

<li><a href="#home">Home</a></li>

<li><a href="#about">About</a></li>

<li><a href="#services">Services</a></li>

<li><a href="#pricing">Pricing</a></li>

<li><a href="#portfolio">Portfolio</a></li>

<li>
<a href="#contact" class="nav-btn">
Contact
</a>
</li>

</ul>

</div>

</nav>


<!-- ================= HERO ================= -->

<section class="hero" id="home">

<div class="container hero-grid">

<div>

<div class="badge">

<i class="fa-solid fa-code"></i>

Professional Web Development

</div>


<h1>

We Create

<span class="gradient-text">
Beautiful Websites
</span>

For Growing Businesses.

</h1>


<p>

Professional WordPress, Elementor,
Business and E-commerce websites
designed to make your business look
professional and attract more customers.

</p>


<div class="buttons">

<a
href="tel:7607627117"
class="btn btn-primary">

<i class="fa-solid fa-phone"></i>

Call Now

</a>


<a
href="https://wa.me/917607627117?text=Hello%20Sachin%20Web%20Solutions%2C%20I%20need%20a%20website."
target="_blank"
class="btn btn-pink">

<i class="fa-brands fa-whatsapp"></i>

WhatsApp

</a>

</div>

</div>


<!-- HERO VISUAL -->

<div class="hero-visual">

<div class="glow-circle"></div>


<div class="web-card">

<div class="browser">

<div class="browser-top">

<div class="browser-dot dot1"></div>

<div class="browser-dot dot2"></div>

<div class="browser-dot dot3"></div>

</div>


<div class="browser-content">

<div class="preview-title"></div>

<div class="preview-line"></div>

<div class="preview-line short"></div>

<div class="preview-line"></div>

<span class="preview-button">
Modern Website
</span>

</div>

</div>

</div>

</div>

</div>

</section>


<!-- ================= ABOUT ================= -->

<section class="about" id="about">

<div class="container about-grid">

<div>

<h2>
Build Your
<span>Digital Presence</span>
With Us.
</h2>

<p>

Sachin Web Solutions creates
modern, responsive and professional
websites for businesses, startups,
local services and entrepreneurs.

</p>

<p>

Our focus is simple — create a website
that looks beautiful, works fast and
helps your business get more customers.

</p>


<div class="about-list">

<div>
<i class="fa-solid fa-check"></i>
Professional Website Design
</div>

<div>
<i class="fa-solid fa-check"></i>
Mobile Responsive
</div>

<div>
<i class="fa-solid fa-check"></i>
WordPress & Elementor
</div>

<div>
<i class="fa-solid fa-check"></i>
Basic SEO Setup
</div>

</div>

</div>


<div class="about-box">

<h3>
Why Does Your Business Need A Website?
</h3>

<p>

Customers are searching online every day.
A professional website helps people
understand your services, contact you
and trust your business.

</p>


<a href="#contact" class="btn btn-pink">

<i class="fa-solid fa-rocket"></i>

Start Your Website

</a>

</div>

</div>

</section>


<!-- ================= SERVICES ================= -->

<section class="services" id="services">

<div class="container">

<div class="section-title">

<h2>
Our Services
</h2>

<p>
Complete digital solutions for your business.
</p>

</div>


<div class="services-grid">


<div class="service-card">

<div class="service-icon blue">
<i class="fa-solid fa-globe"></i>
</div>

<h3>
Business Website
</h3>

<p>
Professional websites for local businesses,
companies and startups.
</p>

</div>


<div class="service-card">

<div class="service-icon purple">
<i class="fa-brands fa-wordpress"></i>
</div>

<h3>
WordPress Website
</h3>

<p>
Modern WordPress websites that are
easy to manage and update.
</p>

</div>


<div class="service-card">

<div class="service-icon pink">
<i class="fa-solid fa-palette"></i>
</div>

<h3>
Elementor Design
</h3>

<p>
Creative Elementor designs with
beautiful responsive layouts.
</p>

</div>


<div class="service-card">

<div class="service-icon orange">
<i class="fa-solid fa-cart-shopping"></i>
</div>

<h3>
E-commerce Website
</h3>

<p>
Online stores designed for products
and growing businesses.
</p>

</div>


<div class="service-card">

<div class="service-icon green">
<i class="fa-solid fa-mobile-screen"></i>
</div>

<h3>
Responsive Design
</h3>

<p>
Perfect experience across mobile,
tablet and desktop devices.
</p>

</div>


<div class="service-card">

<div class="service-icon blue">
<i class="fa-solid fa-magnifying-glass"></i>
</div>

<h3>
Basic SEO
</h3>

<p>
Basic search engine optimization
setup for your website.
</p>

</div>


<div class="service-card">

<div class="service-icon purple">
<i class="fa-solid fa-screwdriver-wrench"></i>
</div>

<h3>
Website Maintenance
</h3>

<p>
Website updates, changes and
ongoing maintenance support.
</p>

</div>


<div class="service-card">

<div class="service-icon orange">
<i class="fa-solid fa-rocket"></i>
</div>

<h3>
Speed Optimization
</h3>

<p>
Improve website performance and
create a faster user experience.
</p>

</div>


</div>

</div>

</section>


<!-- ================= PRICING ================= -->

<section class="pricing" id="pricing">

<div class="container">

<div class="section-title">

<h2>
Website Packages
</h2>

<p>
Choose the package that fits your business.
</p>

</div>


<div class="pricing-grid">


<!-- BASIC -->

<div class="price-card">

<h3>
Basic
</h3>

<div class="price">
₹4,999
</div>

<ul>

<li>✓ 3–5 Pages</li>

<li>✓ Mobile Responsive</li>

<li>✓ WhatsApp Button</li>

<li>✓ Contact Form</li>

<li>✓ Google Map</li>

<li>✓ Basic SEO</li>

</ul>


<a
href="https://wa.me/917607627117?text=Hello%2C%20I%20want%20the%20Basic%20Website%20Package."
target="_blank"
class="btn btn-primary">

<i class="fa-brands fa-whatsapp"></i>

Get Started

</a>

</div>


<!-- PROFESSIONAL -->

<div class="price-card featured">

<div class="popular">
MOST POPULAR
</div>

<h3>
Professional
</h3>

<div class="price">
₹9,999
</div>

<ul>

<li>✓ 5–8 Pages</li>

<li>✓ WordPress + Elementor</li>

<li>✓ Professional Design</li>

<li>✓ WhatsApp Integration</li>

<li>✓ Basic SEO</li>

<li>✓ Speed Optimization</li>

<li>✓ Social Media Integration</li>

</ul>


<a
href="https://wa.me/917607627117?text=Hello%2C%20I%20want%20the%20Professional%20Website%20Package."
target="_blank"
class="btn btn-pink">

<i class="fa-brands fa-whatsapp"></i>

Choose Package

</a>

</div>


<!-- BUSINESS PRO -->

<div class="price-card">

<h3>
Business Pro
</h3>

<div class="price">
₹14,999+
</div>

<ul>

<li>✓ 8–12 Pages</li>

<li>✓ Advanced Design</li>

<li>✓ Lead Generation Forms</li>

<li>✓ Basic SEO Setup</li>

<li>✓ Speed Optimization</li>

<li>✓ Security Setup</li>

<li>✓ 30 Days Support</li>

</ul>


<a
href="https://wa.me/917607627117?text=Hello%2C%20I%20want%20the%20Business%20Pro%20Website%20Package."
target="_blank"
class="btn btn-primary">

<i class="fa-brands fa-whatsapp"></i>

Get Quote

</a>

</div>


</div>

</div>

</section>


<!-- ================= PORTFOLIO ================= -->

<section id="portfolio">

<div class="container">

<div class="section-title">

<h2>
Our Portfolio
</h2>

<p>
Professional website concepts for different businesses.
</p>

</div>


<div class="portfolio-grid">


<div class="project">

<div class="project-img project1">

<i class="fa-solid fa-fire"></i>

</div>

<div class="project-content">

<h3>
Gas Service Website
</h3>

<p>
Professional website for gas appliance
repair and service businesses.
</p>

</div>

</div>


<div class="project">

<div class="project-img project2">

<i class="fa-solid fa-utensils"></i>

</div>

<div class="project-content">

<h3>
Restaurant Website
</h3>

<p>
Modern website design for restaurants
and food businesses.
</p>

</div>

</div>


<div class="project">

<div class="project-img project3">

<i class="fa-solid fa-bag-shopping"></i>

</div>

<div class="project-content">

<h3>
E-commerce Store
</h3>

<p>
Professional online store design
for growing businesses.
</p>

</div>

</div>


</div>

</div>

</section>


<!-- ================= WHY US ================= -->

<section class="why">

<div class="container">

<div class="section-title">

<h2>
Why Choose Sachin Web Solutions?
</h2>

<p>
Professional service with a focus on quality.
</p>

</div>


<div class="why-grid">


<div class="why-card">

<i class="fa-solid fa-bolt"></i>

<strong>
Fast Delivery
</strong>

<p>
Efficient project completion.
</p>

</div>


<div class="why-card">

<i class="fa-solid fa-mobile-screen"></i>

<strong>
Mobile Friendly
</strong>

<p>
Beautiful on every device.
</p>

</div>


<div class="why-card">

<i class="fa-solid fa-bullseye"></i>

<strong>
Business Focused
</strong>

<p>
Designed around your goals.
</p>

</div>


<div class="why-card">

<i class="fa-solid fa-headset"></i>

<strong>
Support
</strong>

<p>
Support after your website goes live.
</p>

</div>


</div>

</div>

</section>


<!-- ================= CONTACT ================= -->

<section class="contact" id="contact">

<div class="container">

<div class="contact-box">

<h2>
Let's Build Something Amazing!
</h2>

<p>
Have a business? Let's create a beautiful
website for your customers.
</p>


<div class="phone">

<i class="fa-solid fa-phone"></i>

7607627117

</div>


<div class="buttons">

<a
href="tel:7607627117"
class="btn btn-primary">

<i class="fa-solid fa-phone"></i>

Call Now

</a>


<a
href="https://wa.me/917607627117?text=Hello%20Sachin%20Web%20Solutions%2C%20I%20want%20to%20build%20a%20website."
target="_blank"
class="btn btn-pink">

<i class="fa-brands fa-whatsapp"></i>

WhatsApp Now

</a>

</div>

</div>

</div>

</section>


<!-- ================= FOOTER ================= -->

<footer>

<div class="container">

<p>

© 2026
<strong>Sachin Web Solutions</strong>.
All Rights Reserved.

</p>

<p>
Professional Web Development Services
</p>

</div>

</footer>


<!-- ================= FLOATING WHATSAPP ================= -->

<a
class="whatsapp"
href="https://wa.me/917607627117?text=Hello%20Sachin%20Web%20Solutions%2C%20I%20need%20a%20website."
target="_blank"
aria-label="WhatsApp">

<i class="fa-brands fa-whatsapp"></i>

</a>


</body>
</html>
