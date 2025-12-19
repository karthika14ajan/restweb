# Ex.06 Restaurant Website
## Date:19/12/2025

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```INDEX.HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Flavor Haven Restaurant</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<!-- HEADER / NAVBAR -->
<header>
    <h1>Flavor Haven</h1>
    <nav>
        <a href="#home">Home</a>
        <a href="#menu">Menu</a>
        <a href="#specials">Specials</a>
        <a href="#ratings">Ratings</a>
        <a href="#gallery">Gallery</a>
        <a href="#offers">Offers</a>
        <a href="#reservation">Reservation</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<!-- HOME -->
<section id="home" class="hero">
    <h2>Delicious Food. Cozy Ambience.</h2>
    <p>Serving happiness on every plate</p>
    <button>Explore Menu</button>
</section>

<!-- MENU -->
<section id="menu" class="menu">
    <h2>Our Menu</h2>

    <div class="menu-grid">
        <div class="menu-card">
            <h3>Butter Chicken</h3>
            <p>Creamy tomato gravy</p>
            <span>₹350</span>
        </div>

        <div class="menu-card">
            <h3>Paneer Tikka</h3>
            <p>Smoky grilled paneer</p>
            <span>₹280</span>
        </div>

        <div class="menu-card">
            <h3>Chicken Biryani</h3>
            <p>Traditional dum biryani</p>
            <span>₹320</span>
        </div
        >

        <div class="menu-card">
            <h3>Pasta Alfredo</h3>
            <p>Creamy Italian pasta</p>
            <span>₹300</span>
        </div>

        <div class="menu-card">
            <h3>Margherita Pizza</h3>
            <p>Cheesy classic pizza</p>
            <span>₹290</span>
        </div>

        <div class="menu-card">
            <h3>Chocolate Lava Cake</h3>
            <p>Molten chocolate dessert</p>
            <span>₹190</span>
        </div>
    </div>
</section>

<!-- SPECIALS -->
<section id="specials" class="section light">
    <h2>Chef’s Specials</h2>
    <p>Handpicked dishes prepared with signature flavors.</p>
    <ul>
        <li>🍛 Royal Chicken Curry</li>
        <li>🥗 Exotic Veg Platter</li>
        <li>🍝 Truffle Cream Pasta</li>
    </ul>
</section>

<!-- RATINGS -->
<section id="ratings" class="section dark">
    <h2>Customer Ratings</h2>
    <p>⭐ 4.6 / 5 (Based on 2,500+ reviews)</p>
    <p>“Amazing taste and great service!”</p>
    <p>“Best restaurant in the city.”</p>
</section>

<!-- GALLERY -->
<section id="gallery" class="section light">
    <h2>Gallery</h2>
    <p>Our ambience and dishes speak for themselves.</p>
    <div class="gallery">
        <div class="box">🍽</div>
        <div class="box">🍕</div>
        <div class="box">🍰</div>
        <div class="box">☕</div>
    </div>
</section>

<!-- OFFERS -->
<section id="offers" class="section dark">
    <h2>Special Offers</h2>
    <ul>
        <li>🎉 20% OFF on weekends</li>
        <li>🍔 Buy 1 Get 1 on Burgers</li>
        <li>🎂 Free dessert on birthdays</li>
    </ul>
</section>

<!-- RESERVATION -->
<section id="reservation" class="section light">
    <h2>Table Reservation</h2>
    <p>Reserve your table by calling us.</p>
    <p>📞 +91 98765 43210</p>
</section>

<!-- CONTACT -->
<section id="contact" class="section contact">
    <h2>Contact Us</h2>
    <p>📍 Chennai, India</p>
    <p>📧 flavorhaven@gmail.com</p>
</section>

<footer>
    © 2025 Flavor Haven Restaurant
</footer>

</body>
</html>
   STYLE.CSS
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

html {
    scroll-behavior: smooth;
}

body {
    background: #f4f4f4;
    color: #333;
}

/* HEADER */
header {
    position: fixed;
    top: 0;
    width: 100%;
    background: #111;
    padding: 15px 40px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 1000;
}

header h1 {
    color: orange;
}

nav a {
    color: white;
    margin-left: 20px;
    text-decoration: none;
    position: relative;
}

nav a::after {
    content: '';
    width: 0;
    height: 2px;
    background: orange;
    position: absolute;
    left: 0;
    bottom: -5px;
    transition: 0.3s;
}

nav a:hover::after {
    width: 100%;
}

/* HERO */
.hero {
    height: 100vh;
    background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)),
    url("https://images.unsplash.com/photo-1552566626-52f8b828add9");
    background-size: cover;
    color: white;
    text-align: center;
    padding-top: 200px;
}

.hero h2 {
    font-size: 45px;
}

.hero button {
    margin-top: 20px;
    padding: 10px 25px;
    background: orange;
    border: none;
    font-size: 16px;
    cursor: pointer;
}

/* SECTIONS */
.section {
    padding: 80px 50px;
    text-align: center;
}

.light {
    background: white;
}

.dark {
    background: #222;
    color: white;
}

.section ul {
    list-style: none;
    margin-top: 20px;
}

.section ul li {
    margin: 10px 0;
}

/* MENU */
.menu {
    padding: 100px 50px;
    background: #fff;
    text-align: center;
}

.menu-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 25px;
    margin-top: 30px;
}

.menu-card {
    background: #fafafa;
    padding: 25px;
    border-radius: 10px;
    box-shadow: 0 4px 10px rgba(0,0,0,0.1);
}

.menu-card h3 {
    color: orange;
}

.menu-card span {
    display: block;
    margin-top: 10px;
    font-weight: bold;
}

/* GALLERY */
.gallery {
    display: flex;
    justify-content: center;
    gap: 20px;
    margin-top: 20px;
}

.box {
    width: 80px;
    height: 80px;
    background: orange;
    font-size: 30px;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 10px;
}

/* CONTACT */
.contact {
    background: orange;
    color: black;
}

/* FOOTER */
footer {
    background: #111;
    color: #aaa;
    text-align: center;
    padding: 15px;
}
```

## OUTPUT:
![alt text](<Screenshot 2025-12-19 134754.png>) ![alt text](<Screenshot 2025-12-19 134808.png>) ![alt text](<Screenshot 2025-12-19 134825.png>) ![alt text](<Screenshot 2025-12-19 134840.png>) ![alt text](<Screenshot 2025-12-19 134924.png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
