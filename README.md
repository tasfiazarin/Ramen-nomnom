

<!DOCTYPE html>

<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Ramen House | Taste of Japan</title>

<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Playfair+Display:wght@600;700;800&display=swap" rel="stylesheet">

<style>

* {

    margin: 0;

    padding: 0;

    box-sizing: border-box;

    scroll-behavior: smooth;

}

:root {

    --red: #c63d25;

    --dark: #241c18;

    --cream: #fff8ed;

    --orange: #e8a34a;

}

body {

    font-family: 'DM Sans', sans-serif;

    background: var(--cream);

    color: var(--dark);

}

header {

    display: flex;

    justify-content: space-between;

    align-items: center;

    padding: 22px 8%;

    background: #fffaf2;

    position: sticky;

    top: 0;

    z-index: 100;

    box-shadow: 0 2px 12px #0000000d;

}

.logo {

    font-family: 'Playfair Display', serif;

    font-size: 28px;

    font-weight: 800;

    color: var(--red);

}

nav a {

    text-decoration: none;

    color: var(--dark);

    margin-left: 25px;

    font-weight: 600;

    transition: .3s;

}

nav a:hover {

    color: var(--red);

}

.hero {

    min-height: 570px;

    display: flex;

    align-items: center;

    padding: 70px 8%;

    background:

    linear-gradient(90deg, #241c18 0%, #241c18dd 45%, #241c1840 100%),

    url('https://images.unsplash.com/photo-1569718212165-3a8278d5f624?auto=format&fit=crop&w=1800&q=85');

    background-size: cover;

    background-position: center;

    color: white;

}

.hero-content {

    max-width: 600px;

}

.hero small {

    color: var(--orange);

    font-weight: bold;

    letter-spacing: 4px;

}

.hero h1 {

    font-family: 'Playfair Display', serif;

    font-size: clamp(45px, 7vw, 76px);

    line-height: 1.1;

    margin: 20px 0;

}

.hero p {

    color: #eee0d4;

    line-height: 1.8;

    margin-bottom: 30px;

    font-size: 16px;

}

.btn {

    display: inline-block;

    background: var(--red);

    color: white;

    padding: 14px 28px;

    text-decoration: none;

    border-radius: 5px;

    font-weight: bold;

    transition: .3s;

}

.btn:hover {

    background: #a52c19;

    transform: translateY(-3px);

}

section {

    padding: 85px 8%;

}

.section-title {

    text-align: center;

    margin-bottom: 45px;

}

.section-title small {

    color: var(--red);

    font-weight: bold;

    letter-spacing: 3px;

}

.section-title h2 {

    font-family: 'Playfair Display', serif;

    font-size: 40px;

    margin-top: 10px;

}

.about {

    display: grid;

    grid-template-columns: 1fr 1fr;

    gap: 55px;

    align-items: center;

}

.about img {

    width: 100%;

    height: 390px;

    object-fit: cover;

    border-radius: 12px;

}

.about-text h2 {

    font-family: 'Playfair Display', serif;

    font-size: 38px;

    margin-bottom: 20px;

}

.about-text p {

    color: #74675d;

    line-height: 1.9;

    margin-bottom: 20px;

}

.types {

    background: #f4eadb;

}

.cards {

    display: grid;

    grid-template-columns: repeat(3, 1fr);

    gap: 25px;

}

.card {

    background: white;

    border-radius: 12px;

    overflow: hidden;

    transition: .3s;

    box-shadow: 0 5px 20px #0000000b;

}

.card:hover {

    transform: translateY(-8px);

    box-shadow: 0 12px 25px #00000015;

}

.card img {

    width: 100%;

    height: 220px;

    object-fit: cover;

}

.card-content {

    padding: 23px;

}

.card-content h3 {

    font-family: 'Playfair Display', serif;

    font-size: 23px;

    margin-bottom: 10px;

}

.card-content p {

    color: #81746a;

    line-height: 1.7;

    font-size: 14px;

}

.menu {

    text-align: center;

}

.menu-list {

    max-width: 750px;

    margin: auto;

}

.menu-item {

    display: flex;

    align-items: center;

    justify-content: space-between;

    padding: 23px 10px;

    border-bottom: 1px dashed #d9c7b4;

    text-align: left;

}

.menu-item h3 {

    font-family: 'Playfair Display', serif;

    font-size: 20px;

}

.menu-item p {

    color: #81746a;

    font-size: 13px;

    margin-top: 6px;

}

.price {

    color: var(--red);

    font-weight: bold;

    font-size: 18px;

    white-space: nowrap;

}

.quote {

    background: var(--dark);

    color: white;

    text-align: center;

    padding: 75px 10%;

}

.quote h2 {

    font-family: 'Playfair Display', serif;

    font-size: 36px;

    margin-bottom: 18px;

}

.quote p {

    color: #e6c9ae;

    line-height: 1.8;

}

.contact {

    text-align: center;

}

.contact p {

    color: #81746a;

    margin: 15px 0 25px;

}

footer {

    background: #17110e;

    color: white;

    text-align: center;

    padding: 30px 15px;

}

footer p {

    color: #c3b3a6;

    font-size: 13px;

    margin-top: 10px;

}

@media(max-width: 800px) {

    header {

        flex-direction: column;

        gap: 15px;

    }

    nav {

        display: flex;

        flex-wrap: wrap;

        justify-content: center;

        gap: 12px;

    }

    nav a {

        margin: 0;

        font-size: 13px;

    }

    .about {

        grid-template-columns: 1fr;

    }

    .cards {

        grid-template-columns: 1fr;

    }

    .hero {

        min-height: 500px;

    }

    section {

        padding: 65px 6%;

    }

}

</style>

</head>

<body>

<header>

    <div class="logo">🍜 RAMEN HOUSE</div>

    <nav>

        <a href="#home">Home</a>

        <a href="#about">About</a>

        <a href="#types">Ramen</a>

        <a href="#menu">Menu</a>

        <a href="#contact">Contact</a>

    </nav>

</header>

<div class="hero" id="home">

    <div class="hero-content">

        <small>AUTHENTIC JAPANESE CUISINE</small>

        <h1>A Bowl Full of Happiness.</h1>

        <p>

            Discover the beautiful world of Japanese ramen.

            Rich broth, handmade noodles, fresh ingredients

            and unforgettable flavors in every single bowl.

        </p>

        <a href="#menu" class="btn">Explore Our Menu</a>

    </div>

</div>

<section class="about" id="about">

    <img src="https://images.unsplash.com/photo-1569718212165-3a8278d5f624?auto=format&fit=crop&w=1000&q=85" alt="Japanese ramen bowl">

    <div class="about-text">

        <small style="color:#c63d25;letter-spacing:3px;font-weight:bold;">

            OUR STORY

        </small>

        <h2>The Art of Japanese Ramen</h2>

        <p>

            Ramen is one of Japan's most loved dishes.

            It is a delicious noodle soup traditionally made

            with wheat noodles, flavorful broth, vegetables,

            meat and carefully selected toppings.

        </p>

        <p>

            From the first sip of warm broth to the last

            bite of noodles, ramen offers a comforting

            experience that brings people together.

        </p>

        <a href="#types" class="btn">Discover Ramen</a>

    </div>

</section>

<section class="types" id="types">

    <div class="section-title">

        <small>EXPLORE THE FLAVORS</small>

        <h2>Our Ramen Collection</h2>

    </div>

    <div class="cards">

        <div class="card">

            <img src="https://images.unsplash.com/photo-1569718212165-3a8278d5f624?auto=format&fit=crop&w=800&q=85" alt="Tonkotsu ramen">

            <div class="card-content">

                <h3>Tonkotsu Ramen</h3>

                <p>A rich and creamy pork-bone broth with tender noodles and delicious toppings.</p>

            </div>

        </div>

        <div class="card">

            <img src="https://images.unsplash.com/photo-1557872943-16a5ac26437e?auto=format&fit=crop&w=800&q=85" alt="Shoyu ramen">

            <div class="card-content">

                <h3>Shoyu Ramen</h3>

                <p>A traditional soy-sauce-based broth with a balanced and savory taste.</p>

            </div>

        </div>

        <div class="card">

            <img src="https://images.unsplash.com/photo-1569050467447-ce54b3bbc37d?auto=format&fit=crop&w=800&q=85" alt="Miso ramen">

            <div class="card-content">

                <h3>Miso Ramen</h3>

                <p>A flavorful fermented soybean paste broth with a deep and comforting taste.</p>

            </div>

        </div>

    </div>

</section>

<section class="menu" id="menu">

    <div class="section-title">

        <small>MADE WITH LOVE</small>

        <h2>Our Special Menu</h2>

    </div>

    <div class="menu-list">

        <div class="menu-item">

            <div>

                <h3>Classic Shoyu Ramen</h3>

                <p>Soy sauce broth, noodles and fresh vegetables</p>

            </div>

            <div class="price">৳450</div>

        </div>

        <div class="menu-item">

            <div>

                <h3>Spicy Miso Ramen</h3>

                <p>Spicy miso broth with delicious toppings</p>

            </div>

            <div class="price">৳520</div>

        </div>

        <div class="menu-item">

            <div>

                <h3>Creamy Tonkotsu</h3>

                <p>Rich broth, noodles and tender meat</p>

            </div>

            <div class="price">৳600</div>

        </div>

        <div class="menu-item">

            <div>

                <h3>Chicken Ramen</h3>

                <p>Chicken broth with egg and vegetables</p>

            </div>

            <div class="price">৳400</div>

        </div>

        <div class="menu-item">

            <div>

                <h3>Vegetable Ramen</h3>

                <p>Fresh vegetables with a flavorful broth</p>

            </div>

            <div class="price">৳350</div>

        </div>

    </div>

</section>

<div class="quote">

    <h2>“Good food. Good mood. Great ramen.”</h2>

    <p>

        Every bowl tells a story of tradition, flavor

        and the beauty of Japanese cuisine.

    </p>

</div>

<section class="contact" id="contact">

    <div class="section-title">

        <small>WE WOULD LOVE TO HEAR FROM YOU</small>

        <h2>Visit Ramen House</h2>

    </div>

    <p>Experience the warmth of authentic Japanese flavors.</p>

    <p><strong>Email:</strong> hello@ramenhouse.com</p>

    <p><strong>Location:</strong> Japan Street, Dhaka, Bangladesh</p>

    <p><strong>Opening Hours:</strong> 11:00 AM – 10:00 PM</p>

    <a href="mailto:hello@ramenhouse.com" class="btn">

        Contact Us

    </a>

</section>

<footer>

    <h2 style="font-family:'Playfair Display',serif;">

        🍜 RAMEN HOUSE

    </h2>

    <p>Bringing the taste of Japan to your table.</p>

    <p>© 2026 Ramen House. All Rights Reserved.</p>

</footer>

</body>

</html>
