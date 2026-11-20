# Commercial_Website1
# Ex02 Commercial Website
## Date:20.11.26

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
```

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TechZone - Commercial Website</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Header -->
    <header>
        <h1>TechZone</h1>
        <p>Your One-Stop Shopping Destination</p>
    </header>

    <!-- Navigation Bar -->
    <nav>
        <a href="#home">Home</a>
        <a href="#products">Products</a>
        <a href="#about">About Us</a>
        <a href="#contact">Contact</a>
        <a href="#account">User Account</a>
    </nav>

    <!-- Home Section -->
    <section id="home" class="hero">
        <h2>Welcome to TechZone</h2>
        <p>Discover the latest technology products at affordable prices.</p>
        <a href="#products" class="btn">Shop Now</a>
    </section>

    <!-- Products Section -->
    <section id="products">
        <h2>Our Products</h2>

        <div class="product-container">

            <div class="product">
                <img src="Strix_G16_KV_16x9.webp"
                     alt="Laptop">
                <h3>Laptop</h3>
                <p>Price: ₹45,000</p>
                <button>Buy Now</button>
            </div>

            <div class="product">
                <img src="A16F8224-F8F7-44F3-A1D5-A9A1AEC9F92D.png"
                     alt="Smartphone">
                <h3>Smartphone</h3>
                <p>Price: ₹20,000</p>
                <button>Buy Now</button>
            </div>

            <div class="product">
                <img src="71noSdO0XjL.jpg"
                     alt="Headphones">
                <h3>Headphones</h3>
                <p>Price: ₹2,000</p>
                <button>Buy Now</button>
            </div>

        </div>
    </section>

    <!-- About Us Section -->
    <section id="about">
        <h2>About Us</h2>
        <p>
            TechZone is an online shopping website that provides
            high-quality electronic products at affordable prices.
            Our goal is to provide customers with the best shopping
            experience.
        </p>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2>Contact Us</h2>
        <p>Email: support@techzone.com</p>
        <p>Phone: +91 9876543210</p>
        <p>Address: Chennai, Tamil Nadu</p>
    </section>

    <!-- User Account Section -->
    <section id="account">
        <h2>User Account</h2>
        <p>Welcome! Login to access your account.</p>
        <button>Login</button>
        <button>Register</button>
    </section>

    <!-- Footer -->
    <footer>
        <p>Follow Us</p>
        <div class="social">
            <a href="https://www.facebook.com/">Facebook</a>
            <a href="https://www.instagram.com/">Instagram</a>
            <a href="https://www.youtube.com/">YouTube</a>
        </div>
        <p>&copy; 2026 TechZone. All Rights Reserved.</p>
    </footer>

</body>
</html>
 style.css 


/* Global Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
    scroll-behavior: smooth;
}

/* Header */
header {
    background-color: #172554;
    color: white;
    text-align: center;
    padding: 25px;
}

/* Navigation Bar */
nav {
    display: flex;
    justify-content: center;
    background-color: #1e40af;
    padding: 15px;
    gap: 30px;
    flex-wrap: wrap;
}

nav a {
    color: white;
    text-decoration: none;
    font-weight: bold;
    transition: 0.3s;
}

nav a:hover {
    color: #facc15;
}

/* Home Section */
.hero {
    background-color: #dbeafe;
    text-align: center;
    padding: 70px 20px;
}

.hero h2 {
    font-size: 32px;
    margin-bottom: 15px;
}

.hero p {
    margin-bottom: 25px;
}

.btn {
    background-color: #2563eb;
    color: white;
    padding: 12px 25px;
    text-decoration: none;
    border-radius: 5px;
}

/* Common Sections */
section {
    padding: 40px 20px;
    text-align: center;
}

section h2 {
    margin-bottom: 25px;
    color: #172554;
}

/* Product Flexbox */
.product-container {
    display: flex;
    justify-content: center;
    align-items: stretch;
    gap: 25px;
    flex-wrap: wrap;
}

.product {
    background-color: #f1f5f9;
    padding: 20px;
    width: 270px;
    border-radius: 10px;
    box-shadow: 0 2px 8px #999;
    transition: transform 0.3s;
}

.product:hover {
    transform: translateY(-8px);
}

.product img {
    width: 100%;
    border-radius: 5px;
}

.product h3 {
    margin: 15px 0;
}

.product p {
    margin-bottom: 15px;
}

/* Buttons */
button {
    background-color: #2563eb;
    color: white;
    border: none;
    padding: 10px 20px;
    border-radius: 5px;
    cursor: pointer;
    margin: 5px;
}

button:hover, .btn:hover {
    background-color: #172554;
}

/* About and Contact */
#about, #contact {
    background-color: #f8fafc;
    line-height: 1.8;
}

/* Footer */
footer {
    background-color: #172554;
    color: white;
    text-align: center;
    padding: 25px;
}

.social {
    display: flex;
    justify-content: center;
    gap: 20px;
    margin: 15px;
    flex-wrap: wrap;
}

.social a {
    color: #facc15;
    text-decoration: none;
}

.social a:hover {
    text-decoration: underline;
}
```
## OUTPUT
![alt text](<EXP-2/Screenshot 2026-11-20 154627.png>)

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.