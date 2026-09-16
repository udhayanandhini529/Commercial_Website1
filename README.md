# Ex02 Commercial Website
## Date:

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
index.html:
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>ShopEase - Commercial Website</title>

    <link rel="stylesheet" href="style.css">
</head>

<body>

    <!-- NAVIGATION BAR -->

    <header>
        <nav class="navbar">

            <h1 class="logo">ShopEase</h1>

            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#products">Products</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>

        </nav>
    </header>


    <!-- HERO SECTION -->

    <section class="hero" id="home">

        <div class="hero-content">

            <h2>Welcome to ShopEase</h2>

            <p>Quality products at affordable prices.</p>

            <button>Shop Now</button>

        </div>

    </section>


    <!-- PRODUCTS SECTION -->

    <section class="products" id="products">

        <h2>Our Products</h2>

        <div class="product-container">


            <!-- PRODUCT 1 -->

            <div class="product-card">

                <img src="https://images.unsplash.com/photo-1546868871-7041f2a55e12?auto=format&fit=crop&w=500&q=80"
                     alt="Smart Watch">

                <h3>Smart Watch</h3>

                <p>₹1,999</p>

                <button>Buy Now</button>

            </div>


            <!-- PRODUCT 2 -->

            <div class="product-card">

                <img src="https://images.unsplash.com/photo-1505740420928-5e560c06d30e?auto=format&fit=crop&w=500&q=80"
                     alt="Headphones">

                <h3>Headphones</h3>

                <p>₹1,499</p>

                <button>Buy Now</button>

            </div>


            <!-- PRODUCT 3 -->

            <div class="product-card">

                <img src="https://images.unsplash.com/photo-1608043152269-423dbba4e7e1?auto=format&fit=crop&w=500&q=80"
                     alt="Wireless Speaker">

                <h3>Wireless Speaker</h3>

                <p>₹2,499</p>

                <button>Buy Now</button>

            </div>


            <!-- PRODUCT 4 -->

            <div class="product-card">

                <img src="https://images.unsplash.com/photo-1511707171634-5f897ff02aa9?auto=format&fit=crop&w=500&q=80"
                     alt="Smart Phone">

                <h3>Smart Phone</h3>

                <p>₹14,999</p>

                <button>Buy Now</button>

            </div>

        </div>

    </section>


    <!-- ABOUT SECTION -->

    <section class="about" id="about">

        <h2>About Us</h2>

        <p>
            ShopEase provides quality products at affordable prices
            with a simple and comfortable shopping experience.
        </p>

    </section>


    <!-- FOOTER -->

    <footer id="contact">

        <h3>ShopEase</h3>

        <p>Email: shopease@gmail.com</p>

        <p>Phone: +91 98765 43210</p>

        <p>© 2026 ShopEase. All Rights Reserved.</p>

    </footer>

</body>

</html>
```

style.css:
```
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
}

body{
    font-family:Arial, sans-serif;
    background:#f5f5f5;
    color:#333;
}


/* NAVIGATION BAR */

header{
    background:#222;
    padding:15px 8%;
}

.navbar{
    display:flex;
    justify-content:space-between;
    align-items:center;
}

.logo{
    color:white;
    font-size:28px;
}

.nav-links{
    display:flex;
    gap:30px;
    list-style:none;
}

.nav-links a{
    color:white;
    text-decoration:none;
    font-size:16px;
}

.nav-links a:hover{
    color:#ff9800;
}


/* HERO SECTION */

.hero{
    min-height:400px;

    display:flex;
    justify-content:center;
    align-items:center;

    text-align:center;

    background:#ffe0b2;

    padding:40px;
}

.hero-content h2{
    font-size:40px;
    margin-bottom:15px;
}

.hero-content p{
    font-size:20px;
    margin-bottom:25px;
}


/* BUTTON */

button{
    border:none;
    padding:12px 25px;

    background:#ff9800;
    color:white;

    border-radius:5px;

    cursor:pointer;
}

button:hover{
    background:#e68900;
}


/* PRODUCTS SECTION */

.products{
    padding:50px 8%;
    text-align:center;
}

.products h2{
    font-size:30px;
    margin-bottom:30px;
}


/* FLEXBOX PRODUCT CONTAINER */

.product-container{

    display:flex;

    justify-content:center;

    align-items:stretch;

    gap:25px;

    flex-wrap:wrap;
}


/* PRODUCT CARD */

.product-card{

    background:white;

    width:220px;

    padding:20px;

    border-radius:10px;

    box-shadow:0 3px 10px rgba(0,0,0,0.1);

    display:flex;

    flex-direction:column;

    align-items:center;

    gap:12px;
}


/* PRODUCT IMAGE */

.product-card img{

    width:100%;

    height:180px;

    object-fit:cover;

    border-radius:8px;
}


.product-card h3{
    font-size:20px;
}

.product-card p{
    font-size:18px;
    font-weight:bold;
}


/* ABOUT SECTION */

.about{

    padding:50px 8%;

    text-align:center;

    background:#fff3e0;
}

.about h2{
    margin-bottom:15px;
}

.about p{
    font-size:17px;
}


/* FOOTER */

footer{

    background:#222;

    color:white;

    text-align:center;

    padding:30px;
}

footer h3{
    margin-bottom:10px;
}

footer p{
    margin:5px;
}


/* RESPONSIVE DESIGN */

@media(max-width:768px){

    .navbar{

        flex-direction:column;

        gap:15px;
    }


    .nav-links{

        flex-direction:column;

        align-items:center;

        gap:12px;
    }


    .hero-content h2{

        font-size:30px;
    }


    .product-container{

        flex-direction:column;

        align-items:center;
    }


    .product-card{

        width:90%;

        max-width:300px;
    }

}
```
## OUTPUT
![alt text](<Screenshot 2026-09-16 110250.png>)
![alt text](<Screenshot (81).png>)
![alt text](<Screenshot 2026-09-16 110325.png>)
## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
