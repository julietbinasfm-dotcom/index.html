
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>IMJHOOOOO | Social Media Management</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Playfair+Display:wght@500;600;700&display=swap');

:root {
    --bg: #faf8f6;
    --white: #ffffff;
    --text: #252322;
    --muted: #77716d;
    --accent: #b98e7a;
    --accent-dark: #8f6857;
    --soft: #eee3dc;
    --border: #e5ddd8;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

body {
    font-family: "DM Sans", sans-serif;
    background: var(--bg);
    color: var(--text);
    line-height: 1.6;
}

a {
    text-decoration: none;
    color: inherit;
}

button {
    font-family: inherit;
}

/* NAVIGATION */

nav {
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 1000;
    background: rgba(250,248,246,.92);
    backdrop-filter: blur(15px);
    border-bottom: 1px solid rgba(229,221,216,.7);
}

.nav-container {
    max-width: 1200px;
    margin: auto;
    padding: 20px 30px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-weight: 700;
    font-size: 21px;
    letter-spacing: 2px;
}

.nav-links {
    display: flex;
    gap: 28px;
    align-items: center;
}

.nav-links a {
    font-size: 14px;
    color: var(--muted);
    transition: .3s;
}

.nav-links a:hover {
    color: var(--accent-dark);
}

.nav-cta {
    background: var(--text);
    color: white !important;
    padding: 11px 19px;
    border-radius: 30px;
}

/* HERO */

.hero {
    min-height: 100vh;
    max-width: 1200px;
    margin: auto;
    padding: 150px 30px 90px;
    display: grid;
    grid-template-columns: 1.2fr .8fr;
    gap: 60px;
    align-items: center;
}

.eyebrow {
    text-transform: uppercase;
    letter-spacing: 3px;
    color: var(--accent-dark);
    font-size: 12px;
    font-weight: 700;
    margin-bottom: 20px;
}

.hero h1 {
    font-family: "Playfair Display", serif;
    font-size: clamp(55px, 7vw, 90px);
    line-height: .98;
    font-weight: 600;
    margin-bottom: 28px;
}

.hero h1 span {
    color: var(--accent);
}

.hero p {
    max-width: 570px;
    color: var(--muted);
    font-size: 18px;
    margin-bottom: 35px;
}

.buttons {
    display: flex;
    gap: 14px;
    flex-wrap: wrap;
}

.btn {
    padding: 14px 24px;
    border-radius: 30px;
    border: 1px solid var(--text);
    font-weight: 600;
    cursor: pointer;
    transition: .3s;
}

.btn-primary {
    background: var(--text);
    color: white;
}

.btn-primary:hover {
    transform: translateY(-3px);
}

.btn-secondary {
    background: transparent;
}

.btn-secondary:hover {
    background: var(--soft);
}

.hero-card {
    background: var(--soft);
    border-radius: 35px;
    padding: 45px;
    min-height: 470px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

.hero-card .big-text {
    font-family: "Playfair Display", serif;
    font-size: 55px;
    line-height: 1;
}

.hero-card-bottom {
    border-top: 1px solid rgba(0,0,0,.12);
    padding-top: 25px;
    color: var(--muted);
}

/* GENERAL */

section {
    padding: 100px 30px;
}

.section-container {
    max-width: 1200px;
    margin: auto;
}

.section-label {
    color: var(--accent-dark);
    text-transform: uppercase;
    letter-spacing: 2px;
    font-size: 12px;
    font-weight: 700;
    margin-bottom: 12px;
}

.section-title {
    font-family: "Playfair Display", serif;
    font-size: 48px;
    line-height: 1.1;
    margin-bottom: 50px;
}

/* SERVICES */

.services {
    background: white;
}

.service-grid {
    display: grid;
    grid-template-columns: repeat(3,1fr);
    gap: 18px;
}

.service {
    border: 1px solid var(--border);
    border-radius: 22px;
    padding: 32px;
    transition: .3s;
    cursor: pointer;
}

.service:hover {
    transform: translateY(-7px);
    border-color: var(--accent);
}

.service-number {
    color: var(--accent);
    font-weight: 700;
    margin-bottom: 35px;
}

.service h3 {
    margin-bottom: 12px;
    font-size: 20px;
}

.service p {
    color: var(--muted);
    font-size: 14px;
}

/* PORTFOLIO */

.portfolio-filter {
    display: flex;
    gap: 10px;
    margin-bottom: 35px;
    flex-wrap: wrap;
}

.filter {
    border: 1px solid var(--border);
    background: transparent;
    padding: 10px 18px;
    border-radius: 25px;
    cursor: pointer;
}

.filter.active,
.filter:hover {
    background: var(--text);
    color: white;
}

.portfolio-grid {
    display: grid;
    grid-template-columns: repeat(3,1fr);
    gap: 20px;
}

.project {
    background: white;
    border: 1px solid var(--border);
    border-radius: 25px;
    overflow: hidden;
    transition: .3s;
}

.project:hover {
    transform: translateY(-5px);
}

.project-image {
    height: 240px;
    background: var(--soft);
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: "Playfair Display", serif;
    font-size: 28px;
}

.project-info {
    padding: 24px;
}

.project-info small {
    color: var(--accent-dark);
    text-transform: uppercase;
    letter-spacing: 1px;
}

.project-info h3 {
    margin: 8px 0;
}

.project-info p {
    color: var(--muted);
    font-size: 14px;
}

/* CONTENT WITH A PURPOSE BACKGROUND */

#portfolio {
    background:
        linear-gradient(rgba(250,248,246,.86), rgba(250,248,246,.92)),
        url('https://uploads.onecompiler.io/4534xvdks/4534y479v/content.jpg') center/cover fixed;
}

/* CONTENT PLANNER */

.planner {
    background: var(--text);
    color: white;
}

.planner .section-label {
    color: #d7b5a3;
}

.planner .section-title {
    color: white;
}

.calendar {
    display: grid;
    grid-template-columns: repeat(5,1fr);
    gap: 10px;
}

.day {
    background: #302e2c;
    padding: 22px;
    border-radius: 18px;
    min-height: 170px;
    border: 1px solid #45413e;
}

.day span {
    color: #d7b5a3;
    font-size: 11px;
    font-weight: 700;
}

.day h4 {
    margin: 12px 0;
}

.day p {
    color: #aaa5a1;
    font-size: 13px;
}

/* PROCESS */

.process-grid {
    display: grid;
    grid-template-columns: repeat(5,1fr);
    gap: 12px;
}

.process {
    padding: 25px;
    border-top: 2px solid var(--accent);
}

.process strong {
    font-size: 12px;
    color: var(--accent-dark);
}

.process h3 {
    margin: 15px 0 8px;
}

.process p {
    color: var(--muted);
    font-size: 13px;
}

/* PRICING */

.pricing {
    background: white;
}

.price-grid {
    display: grid;
    grid-template-columns: repeat(3,1fr);
    gap: 20px;
}

.price-card {
    border: 1px solid var(--border);
    border-radius: 25px;
    padding: 35px;
}

.price-card.featured {
    background: var(--text);
    color: white;
    transform: translateY(-10px);
}

.price-card small {
    color: var(--accent);
    text-transform: uppercase;
    letter-spacing: 2px;
}

.price-card h3 {
    font-size: 25px;
    margin: 15px 0;
}

.price {
    font-family: "Playfair Display", serif;
    font-size: 42px;
    margin-bottom: 25px;
}

.price-card ul {
    list-style: none;
    margin-bottom: 30px;
}

.price-card li {
    padding: 8px 0;
    color: var(--muted);
    border-bottom: 1px solid var(--border);
}

.featured li {
    color: #c7c1bd;
    border-color: #44403d;
}

/* ABOUT */

.about-grid {
    display: grid;
    grid-template-columns: .8fr 1.2fr;
    gap: 70px;
    align-items: center;
}

.about-box {
    background: var(--soft);
    min-height: 400px;
    border-radius: 30px;
    display: flex;
    justify-content: center;
    align-items: center;
}

.about-box strong {
    font-family: "Playfair Display", serif;
    font-size: 55px;
}

.about-text h2 {
    font-family: "Playfair Display", serif;
    font-size: 50px;
    line-height: 1.1;
    margin-bottom: 25px;
}

.about-text p {
    color: var(--muted);
    margin-bottom: 20px;
}

/* CONTACT */

.contact {
    background: var(--soft);
    text-align: center;
}

.contact .section-title {
    margin-bottom: 20px;
}

.contact p {
    color: var(--muted);
    max-width: 600px;
    margin: 0 auto 30px;
}

.contact-links {
    display: flex;
    justify-content: center;
    gap: 15px;
    flex-wrap: wrap;
}

/* FOOTER */

footer {
    padding: 30px;
    background: var(--text);
    color: #aaa5a1;
    text-align: center;
    font-size: 13px;
}

/* ATTACHED EDITORIAL IMAGERY */

.hero-card {
    background: #d9d5ce;
    min-height: 520px;
    padding: 0;
    isolation: isolate;
}

.hero-card img {
    position: absolute;
    inset: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: center;
    opacity: .92;
}

.hero-card > div {
    padding: 45px;
}

.hero-card::after {
    content: "";
    position: absolute;
    inset: 0;
    border-radius: inherit;
    background: linear-gradient(180deg, rgba(25,22,20,.08), rgba(25,22,20,.58));
    z-index: 0;
}

.project-image {
    background-size: cover;
    background-position: center;
    min-height: 290px;
}

.project-image::before {
    z-index: 1;
}

.project-image::after {
    z-index: 1;
}

.service:nth-child(1),
.service:nth-child(4) {
    background: linear-gradient(90deg, rgba(255,255,255,.96), rgba(255,255,255,.75)), url('How to build the perfect florist website - step-by-step guide — Gem Media.jpg') center/cover;
}

.service:nth-child(2),
.service:nth-child(5) {
    background: linear-gradient(90deg, rgba(255,255,255,.96), rgba(255,255,255,.75)), url('Maximize Your Business Growth with Hey V_A - Your Ultimate Virtual Business Support.jpg') center/cover;
}

.service:nth-child(3),
.service:nth-child(6) {
    background: linear-gradient(90deg, rgba(255,255,255,.96), rgba(255,255,255,.75)), url('How to Build a Personal Brand_ Simple Tips to Stand Out Online.jpg') center/cover;
}

.planner {
    background: linear-gradient(90deg, rgba(37,35,34,.98), rgba(37,35,34,.84)), url('download (7).jpg') center 35%/cover;
}

.price-card {
    background: linear-gradient(145deg, rgba(255,255,255,.96), rgba(238,227,220,.86)), url('How to Build a Personal Brand_ Simple Tips to Stand Out Online.jpg') center/cover;
}

.price-card.featured {
    background: linear-gradient(145deg, rgba(37,35,34,.98), rgba(37,35,34,.84)), url('Maximize Your Business Growth with Hey V_A - Your Ultimate Virtual Business Support.jpg') center/cover;
}

/* GRAPHICS & VISUAL DETAILS */

.hero-card {
    position: relative;
    overflow: hidden;
}

.hero-card::before,
.hero-card::after {
    content: "";
    position: absolute;
    border-radius: 50%;
    pointer-events: none;
}

.hero-card::before {
    width: 230px;
    height: 230px;
    right: -65px;
    top: 105px;
    background: rgba(185,142,122,.45);
}

.hero-card::after {
    width: 145px;
    height: 145px;
    right: 72px;
    top: 165px;
    border: 1px solid rgba(143,104,87,.55);
}

.hero-card > div {
    position: relative;
    z-index: 1;
}

.service {
    position: relative;
    overflow: hidden;
}

.service::after {
    content: "✦";
    position: absolute;
    right: 22px;
    bottom: 14px;
    color: var(--soft);
    font-size: 58px;
    line-height: 1;
    transition: .3s;
}

.service:hover::after {
    color: var(--accent);
    transform: rotate(18deg) scale(1.1);
}

.graphic-label {
    position: relative;
    z-index: 1;
    letter-spacing: 2px;
}

    .project-image {
    position: relative;
    overflow: hidden;
    aspect-ratio: 1 / 1;
    min-height: 0;
    background: linear-gradient(135deg, #eee3dc 0%, #d7b5a3 100%);
}

.project-image .graphic-label {
    position: relative;
    z-index: 2;
}

.project-image::before,
.project-image::after {
    content: "";
    position: absolute;
    border-radius: 50%;
    opacity: .8;
}

.project-image::before {
    width: 150px;
    height: 150px;
    background: rgba(255,255,255,.48);
    top: -45px;
    right: -20px;
}

.project-image::after {
    width: 95px;
    height: 95px;
    background: var(--accent-dark);
    bottom: -40px;
    left: 30px;
}

.project-image {
    color: var(--text);
}

.project-image::first-line {
    position: relative;
}

.project-image + .project-info {
    position: relative;
}

.day,
.process,
.price-card,
.about-box {
    position: relative;
    overflow: hidden;
}

.day::after {
    content: "";
    position: absolute;
    width: 70px;
    height: 70px;
    right: -18px;
    bottom: -20px;
    border: 1px solid rgba(215,181,163,.45);
    border-radius: 50%;
}

.process::after {
    content: "→";
    position: absolute;
    right: 16px;
    top: 18px;
    color: var(--soft);
    font-size: 28px;
}

.price-card::before {
    content: "";
    position: absolute;
    width: 90px;
    height: 90px;
    top: -48px;
    right: -25px;
    border-radius: 50%;
    background: var(--soft);
}

.price-card.featured::before {
    background: #45413e;
}

.about-box {
    background: linear-gradient(145deg, var(--soft), #d7b5a3);
}

.about-box img {
    position: absolute;
    inset: 0;
    z-index: 1;
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: center top;
    opacity: 1;
    mix-blend-mode: normal;
}

.about-box::before,
.about-box::after {
    content: "";
    position: absolute;
    border: 1px solid rgba(143,104,87,.55);
    transform: rotate(25deg);
}

.about-box::before {
    width: 220px;
    height: 280px;
    border-radius: 50%;
}

.about-box::after {
    width: 150px;
    height: 150px;
    border-radius: 50%;
}

.about-box strong {
    position: relative;
    z-index: 1;
}

.contact {
    position: relative;
    overflow: hidden;
}

.contact::before,
.contact::after {
    content: "";
    position: absolute;
    border: 1px solid rgba(143,104,87,.3);
    border-radius: 50%;
    pointer-events: none;
}

.contact::before {
    width: 280px;
    height: 280px;
    left: -125px;
    top: 35px;
}

.contact::after {
    width: 190px;
    height: 190px;
    right: -80px;
    bottom: -70px;
}

.contact .section-container {
    position: relative;
    z-index: 1;
}

/* MOBILE */

@media(max-width: 800px) {

    .nav-links {
        display: none;
    }

    .hero {
        grid-template-columns: 1fr;
        padding-top: 130px;
    }

    .hero-card {
        min-height: 330px;
    }

    .service-grid,
    .portfolio-grid,
    .price-grid {
        grid-template-columns: 1fr;
    }

    .calendar {
        grid-template-columns: 1fr;
    }

    .process-grid {
        grid-template-columns: 1fr 1fr;
    }

    .about-grid {
        grid-template-columns: 1fr;
    }

    .section-title {
        font-size: 38px;
    }

    .hero h1 {
        font-size: 58px;
    }
}
</style>
</head>

<body>

<!-- NAVIGATION -->

<nav>
<div class="nav-container">

<a href="#home" class="logo">IMJHOOOOO</a>

<div class="nav-links">
<a href="#services">Services</a>
<a href="#portfolio">Portfolio</a>
<a href="#planner">Planner</a>
<a href="#process">Process</a>
<a href="#pricing">Packages</a>
<a href="#about">About</a>
<a href="#contact" class="nav-cta">Let's Work</a>
</div>

</div>
</nav>


<!-- HERO -->

<section class="hero" id="home">

<div>

<div class="eyebrow">
Social Media Management • UGC • Content
</div>

<h1>
Make your brand<br>
<span>impossible</span><br>
to scroll past.
</h1>

<p>
I help brands create strategic, authentic and
scroll-stopping social media content that turns
attention into connection—and connection into customers.
</p>

<div class="buttons">
<a href="#portfolio" class="btn btn-primary">
View My Work →
</a>

<a href="#contact" class="btn btn-secondary">
Work With Me
</a>
</div>

</div>

<div class="hero-card">

<div>
<div class="eyebrow">What I do</div>

<div class="big-text">
Strategy.<br>
Content.<br>
Growth.
</div>
</div>

<div class="hero-card-bottom">
From content planning to UGC and social media
management, I create content designed to feel
human—not overly promotional.
</div>

</div>

</section>


<!-- SERVICES -->

<section class="services" id="services">

<div class="section-container">

<div class="section-label">What I offer</div>

<h2 class="section-title">
Social media support<br>
that actually has a strategy.
</h2>

<div class="service-grid">

<div class="service">
<div class="service-number">01</div>
<h3>Social Media Management</h3>
<p>
Content scheduling, publishing, platform management,
engagement and maintaining your brand's online presence.
</p>
</div>

<div class="service">
<div class="service-number">02</div>
<h3>Content Strategy</h3>
<p>
Content pillars, monthly calendars, campaign ideas,
hooks and platform-specific content planning.
</p>
</div>

<div class="service">
<div class="service-number">03</div>
<h3>UGC Content</h3>
<p>
Authentic short-form videos that make products feel
relatable, trustworthy and worth trying.
</p>
</div>

<div class="service">
<div class="service-number">04</div>
<h3>Copywriting</h3>
<p>
Scroll-stopping hooks, captions, CTAs and product
copy designed to communicate clearly.
</p>
</div>

<div class="service">
<div class="service-number">05</div>
<h3>Community Management</h3>
<p>
Comment and message engagement that keeps your
audience connected to your brand.
</p>
</div>

<div class="service">
<div class="service-number">06</div>
<h3>Analytics & Reporting</h3>
<p>
Performance tracking and insights to understand
what works and improve future content.
</p>
</div>

</div>
</div>
</section>


<!-- PORTFOLIO -->

<section id="portfolio">

<div class="section-container">

<div class="section-label">Selected work</div>

<h2 class="section-title">
Content with a purpose.
</h2>

<div class="portfolio-filter">

<button class="filter active" onclick="filterProjects('all', this)">
All
</button>

<button class="filter" onclick="filterProjects('ugc', this)">
UGC
</button>

<button class="filter" onclick="filterProjects('strategy', this)">
Strategy
</button>

<button class="filter" onclick="filterProjects('beauty', this)">
Beauty
</button>

</div>

<div class="portfolio-grid">

<div class="project" data-category="beauty ugc">
<div class="project-image">
<span class="graphic-label">SKINCARE</span>
</div>
<div class="project-info">
<small>UGC Campaign</small>
<h3>Everyday Skincare</h3>
<p>
Authentic routine-based content designed
to introduce the product naturally.
</p>
</div>
</div>

<div class="project" data-category="strategy">
<div class="project-image">
<span class="graphic-label">CONTENT</span>
</div>
<div class="project-info">
<small>Strategy</small>
<h3>30-Day Content System</h3>
<p>
A balanced content strategy combining
education, lifestyle and conversion posts.
</p>
</div>
</div>

<div class="project" data-category="beauty">
<div class="project-image">
<span class="graphic-label">BEAUTY</span>
</div>
<div class="project-info">
<small>Social Campaign</small>
<h3>Beauty Brand Launch</h3>
<p>
A campaign concept built around awareness,
trust and product discovery.
</p>
</div>
</div>

<div class="project" data-category="ugc beauty">
<div class="project-image">
<span class="graphic-label">REVIEW</span>
</div>
<div class="project-info">
<small>UGC</small>
<h3>Honest Product Review</h3>
<p>
A creator-style review focused on experience,
texture and realistic product benefits.
</p>
</div>
</div>

<div class="project" data-category="strategy">
<div class="project-image" style="background-image: url('How to build the perfect florist website - step-by-step guide — Gem Media.jpg');">
<span class="graphic-label">SOCIAL</span>
</div>
<div class="project-info">
<small>Strategy</small>
<h3>Social Media Refresh</h3>
<p>
Content pillars and posting rhythm designed
to create a stronger brand identity.
</p>
</div>
</div>

<div class="project" data-category="ugc">
<div class="project-image" style="background-image: url('Maximize Your Business Growth with Hey V_A - Your Ultimate Virtual Business Support.jpg');">
<span class="graphic-label">GRWM</span>
</div>
<div class="project-info">
<small>UGC</small>
<h3>GRWM Campaign</h3>
<p>
Lifestyle-led content integrating products
into a natural everyday routine.
</p>
</div>
</div>

</div>
</div>
</section>


<!-- CONTENT PLANNER -->

<section class="planner" id="planner">

<div class="section-container">

<div class="section-label">Sample content planner</div>

<h2 class="section-title">
A month of content,<br>
planned with intention.
</h2>

<div class="calendar">

<div class="day">
<span>MONDAY</span>
<h4>Educate</h4>
<p>Skincare tips, ingredients, FAQs and saveable content.</p>
</div>

<div class="day">
<span>TUESDAY</span>
<h4>UGC</h4>
<p>GRWM, routines, voiceovers and authentic product integration.</p>
</div>

<div class="day">
<span>WEDNESDAY</span>
<h4>Proof</h4>
<p>Reviews, texture shots, wear tests and experiences.</p>
</div>

<div class="day">
<span>THURSDAY</span>
<h4>Relate</h4>
<p>POVs, trends, relatable skincare moments and storytelling.</p>
</div>

<div class="day">
<span>FRIDAY</span>
<h4>Convert</h4>
<p>Product highlights, bundles, testimonials and CTAs.</p>
</div>

</div>

</div>
</section>


<!-- PROCESS -->

<section id="process">

<div class="section-container">

<div class="section-label">My process</div>

<h2 class="section-title">
From idea to execution.
</h2>

<div class="process-grid">

<div class="process">
<strong>01</strong>
<h3>Discover</h3>
<p>Understand your brand, audience and goals.</p>
</div>

<div class="process">
<strong>02</strong>
<h3>Strategize</h3>
<p>Build content pillars and a clear posting plan.</p>
</div>

<div class="process">
<strong>03</strong>
<h3>Create</h3>
<p>Develop content, UGC, captions and creative concepts.</p>
</div>

<div class="process">
<strong>04</strong>
<h3>Publish</h3>
<p>Schedule, publish and maintain consistency.</p>
</div>

<div class="process">
<strong>05</strong>
<h3>Optimize</h3>
<p>Review performance and improve the strategy.</p>
</div>

</div>

</div>
</section>


<!-- PRICING -->

<section class="pricing" id="pricing">

<div class="section-container">

<div class="section-label">Work with me</div>

<h2 class="section-title">
Choose your level of support.
</h2>

<div class="price-grid">

<div class="price-card">

<small>Starter</small>
<h3>Content Support</h3>

<div class="price">
Custom
</div>

<ul>
<li>Content ideas</li>
<li>Monthly content calendar</li>
<li>Caption & hook ideas</li>
<li>Content planning</li>
</ul>

<a href="#contact" class="btn btn-secondary">
Inquire →
</a>

</div>


<div class="price-card featured">

<small>Most Popular</small>
<h3>Social Growth</h3>

<div class="price">
Custom
</div>

<ul>
<li>Content strategy</li>
<li>Monthly content calendar</li>
<li>Social media management</li>
<li>UGC content support</li>
<li>Community engagement</li>
<li>Monthly analytics</li>
</ul>

<a href="#contact" class="btn btn-primary">
Let's Talk →
</a>

</div>


<div class="price-card">

<small>Premium</small>
<h3>Full Management</h3>

<div class="price">
Custom
</div>

<ul>
<li>Full social media management</li>
<li>Content strategy</li>
<li>UGC creation</li>
<li>Copywriting</li>
<li>Community management</li>
<li>Performance reporting</li>
</ul>

<a href="#contact" class="btn btn-secondary">
Inquire →
</a>

</div>

</div>
</div>
</section>


<!-- ABOUT -->

<section id="about">

<div class="section-container about-grid">

<div class="about-box">
<img src="https://uploads.onecompiler.io/4534xvdks/4534y479v/founder.png" alt="Portrait of the founder">
</div>

<div class="about-text">

<div class="section-label">About me</div>

<h2>
Behind the content is a strategy.
</h2>

<p>
I'm a content creator and social media-focused virtual
professional who enjoys turning simple ideas into
content people actually want to watch.
</p>

<p>
My approach combines creativity with organization:
planning content intentionally, creating relatable
UGC, writing clear copy and paying attention to
what the audience responds to.
</p>

<a href="#contact" class="btn btn-primary">
Let's Create Together →
</a>

</div>

</div>
</section>


<!-- CONTACT -->

<section class="contact" id="contact">

<div class="section-container">

<div class="section-label">Let's work together</div>

<h2 class="section-title">
Ready to make your<br>
brand more social?
</h2>

<p>
Tell me about your brand, your goals and what you
need help with. Let's build something your audience
will actually remember.
</p>

<div class="contact-links">

<a href="mailto:hello@imjhooooo.com" class="btn btn-primary">
Email Me
</a>

<a href="https://www.tiktok.com/" target="_blank" class="btn btn-secondary">
TikTok →
</a>

<a href="https://www.instagram.com/" target="_blank" class="btn btn-secondary">
Instagram →
</a>

</div>

</div>
</section>


<footer>
© 2026 IMJHOOOOO • Social Media Management • UGC • Content Strategy
</footer>


<script>

/* PORTFOLIO FILTER */

function filterProjects(category, button) {

    const projects = document.querySelectorAll(".project");
    const filters = document.querySelectorAll(".filter");

    filters.forEach(filter => {
        filter.classList.remove("active");
    });

    button.classList.add("active");

    projects.forEach(project => {

        if(category === "all") {
            project.style.display = "block";
        }

        else if(project.dataset.category.includes(category)) {
            project.style.display = "block";
        }

        else {
            project.style.display = "none";
        }

    });
}


/* NAVIGATION ACTIVE EFFECT */

const sections = document.querySelectorAll("section");
const navLinks = document.querySelectorAll(".nav-links a");

window.addEventListener("scroll", () => {

    let current = "";

    sections.forEach(section => {

        const sectionTop = section.offsetTop - 150;

        if(window.scrollY >= sectionTop) {
            current = section.getAttribute("id");
        }

    });

    navLinks.forEach(link => {

        link.style.color = "";

        if(link.getAttribute("href") === "#" + current) {
            link.style.color = "#8f6857";
        }

    });

});

</script>

</body>
</html>
