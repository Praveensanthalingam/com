# Ex02 Commercial Website
## Date:21.11.2026

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
INDEX


  ```
  <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aurelia Footwear | Commercial Storefront</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Navigation Bar -->
    <header class="navbar">
        <div class="logo">AURELIA</div>
        <nav class="nav-links">
            <a href="#home">Home</a>
            <a href="#products">Collection</a>
            <a href="#about">Craftsmanship</a>
            <a href="#footer">Contact</a>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <h1>Handcrafted Comfort, Modern Silhouette</h1>
        <p>Explore artisanal footwear designed for everyday elegance.</p>
        <a href="#products" class="btn-primary">Shop Now</a>
    </section>

    <!-- Product Showcase Section -->
    <main id="products" class="product-section">
        <h2 class="section-title">Featured Collection</h2>
        
        <div class="product-container">
            <!-- Product 1 -->
            <article class="product-card">
                <img src="https://via.placeholder.com/300x220/e8dfd5/333333?text=Embroidered+Jooti" alt="Royal Zari Jooti">
                <div class="card-body">
                    <h3>Royal Zari Jooti</h3>
                    <p class="description">Hand-stitched velvet upper with cushioned leather sole.</p>
                    <div class="card-footer">
                        <span class="price">₹1,899</span>
                        <button class="btn-cart">Add to Cart</button>
                    </div>
                </div>
            </article>

            <!-- Product 2 -->
            <article class="product-card">
                <img src="https://via.placeholder.com/300x220/d5e0e8/333333?text=Pastel+Mule" alt="Indigo Fusion Mule">
                <div class="card-body">
                    <h3>Indigo Fusion Mule</h3>
                    <p class="description">Minimalist woven pattern ideal for casual and festive wear.</p>
                    <div class="card-footer">
                        <span class="price">₹1,599</span>
                        <button class="btn-cart">Add to Cart</button>
                    </div>
                </div>
            </article>

            <!-- Product 3 -->
            <article class="product-card">
                <img src="https://via.placeholder.com/300x220/e8d5d8/333333?text=Classic+Loafer" alt="Terracotta Tan Loafer">
                <div class="card-body">
                    <h3>Terracotta Tan Loafer</h3>
                    <p class="description">Breathable vegan leather with ergonomic arch support.</p>
                    <div class="card-footer">
                        <span class="price">₹2,199</span>
                        <button class="btn-cart">Add to Cart</button>
                    </div>
                </div>
            </article>

            <!-- Product 4 -->
            <article class="product-card">
                <img src="https://via.placeholder.com/300x220/d8e8d5/333333?text=Festive+Edition" alt="Emerald Silk Slip-On">
                <div class="card-body">
                    <h3>Emerald Silk Slip-On</h3>
                    <p class="description">Raw silk finish accented with subtle metallic threadwork.</p>
                    <div class="card-footer">
                        <span class="price">₹2,499</span>
                        <button class="btn-cart">Add to Cart</button>
                    </div>
                </div>
            </article>
        </div>
    </main>

    <!-- Footer Section -->
    <footer id="footer" class="footer">
        <div class="footer-col">
            <h4>AURELIA STORE</h4>
            <p>Delivering handcrafted quality nationwide.</p>
        </div>
        
        <div class="footer-col student-info">
            <h4>Developed By</h4>
            <!-- Replace with your actual Name and Register Number -->
            <p><strong>Name:</strong> PRAVEEN</p>
            <p><strong>Register No:</strong>212224040246</p>
        </div>

        <div class="footer-col">
            <h4>Customer Care</h4>
            <p>Email: support@aureliastore.in</p>
            <p>&copy; 2026 Aurelia Footwear</p>
        </div>
    </footer>

</body>
</html>
  ```
Style

```
/* Global Reset & Base Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

body {
    background-color: #f9f8f6;
    color: #222222;
    display: flex;
    flex-direction: column;
    min-height: 100vh;
}

/* 1. Navigation Bar (Flexbox Row) */
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #1e1e24;
    color: #ffffff;
    padding: 1rem 5%;
    position: sticky;
    top: 0;
    z-index: 100;
}

.logo {
    font-size: 1.5rem;
    font-weight: 700;
    letter-spacing: 2px;
    color: #e0a96d;
}

.nav-links {
    display: flex;
    gap: 1.5rem;
}

.nav-links a {
    color: #ffffff;
    text-decoration: none;
    font-size: 0.95rem;
    transition: color 0.3s ease;
}

.nav-links a:hover {
    color: #e0a96d;
}

/* 2. Hero Section (Flexbox Column Centering) */
.hero {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    background: linear-gradient(135deg, #2b2d42, #1e1e24);
    color: #ffffff;
    padding: 4rem 1.5rem;
    gap: 1rem;
}

.hero h1 {
    font-size: 2.4rem;
    max-width: 700px;
}

.hero p {
    font-size: 1.1rem;
    color: #cccccc;
}

.btn-primary {
    margin-top: 0.5rem;
    padding: 0.75rem 1.75rem;
    background-color: #e0a96d;
    color: #1e1e24;
    text-decoration: none;
    font-weight: 600;
    border-radius: 4px;
    transition: background-color 0.3s ease;
}

.btn-primary:hover {
    background-color: #cf9455;
}

/* 3. Product Grid Section (Responsive Flex Wrapping) */
.product-section {
    padding: 3rem 5%;
    flex: 1;
}

.section-title {
    text-align: center;
    font-size: 1.8rem;
    margin-bottom: 2rem;
    color: #1e1e24;
}

.product-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1.5rem;
}

.product-card {
    background-color: #ffffff;
    border-radius: 8px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
    overflow: hidden;
    /* Flex shorthand: grow=1, shrink=1, basis=260px */
    flex: 1 1 260px;
    max-width: 320px;
    display: flex;
    flex-direction: column;
    transition: transform 0.25s ease;
}

.product-card:hover {
    transform: translateY(-5px);
}

.product-card img {
    width: 100%;
    height: 200px;
    object-fit: cover;
}

.card-body {
    padding: 1.25rem;
    display: flex;
    flex-direction: column;
    flex: 1;
    justify-content: space-between;
}

.card-body h3 {
    font-size: 1.2rem;
    margin-bottom: 0.5rem;
}

.description {
    font-size: 0.9rem;
    color: #555555;
    margin-bottom: 1.25rem;
    line-height: 1.4;
}

.card-footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-top: 1px solid #eeeeee;
    padding-top: 0.75rem;
}

.price {
    font-size: 1.15rem;
    font-weight: 700;
    color: #1e1e24;
}

.btn-cart {
    padding: 0.5rem 1rem;
    background-color: #1e1e24;
    color: #ffffff;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    font-size: 0.9rem;
}

.btn-cart:hover {
    background-color: #e0a96d;
    color: #1e1e24;
}

/* 4. Footer Section */
.footer {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    background-color: #1e1e24;
    color: #dddddd;
    padding: 2rem 5%;
    gap: 1.5rem;
}

.footer-col {
    flex: 1 1 220px;
}

.footer-col h4 {
    color: #e0a96d;
    margin-bottom: 0.75rem;
    font-size: 1rem;
}

.footer-col p {
    font-size: 0.9rem;
    line-height: 1.6;
}

/* Media Query for Mobile Viewports */
@media (max-width: 650px) {
    .navbar {
        flex-direction: column;
        gap: 1rem;
    }

    .nav-links {
        flex-wrap: wrap;
        justify-content: center;
    }

    .hero h1 {
        font-size: 1.8rem;
    }

    .footer {
        flex-direction: column;
        text-align: center;
    }
}
```

## OUTPUT
<img width="1918" height="1091" alt="image" src="https://github.com/user-attachments/assets/8ea5bbf4-182d-45d5-97b7-34556c4e6663" />


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
