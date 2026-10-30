# Ex02 Commercial Website
## Date:30-10-2026

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
## HTML
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>UrbanNest | Home & Lifestyle Store</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
 
  <!-- HEADER + NAVIGATION -->
  <header class="site-header">
    <div class="container nav-wrap">
      <a href="#home" class="logo">Urban<span>Nest</span></a>
      <nav>
        <ul class="nav-links">
          <li><a href="#home">Home</a></li>
          <li><a href="#products">Products</a></li>
          <li><a href="#about">About Us</a></li>
          <li><a href="#contact">Contact</a></li>
          <li><a href="#account" class="btn btn-small">My Account</a></li>
        </ul>
      </nav>
    </div>
  </header>
 
  <main>
    <!-- HOMEPAGE -->
    <section id="home" class="hero">
      <div class="container hero-inner">
        <div class="hero-text">
          <p class="eyebrow">New Season Collection</p>
          <h1>Make Every Room Feel Like Home</h1>
          <p>Thoughtfully designed furniture, decor and lighting delivered to your door, with free shipping on orders above ₹2,999.</p>
          <a href="#products" class="btn">Shop Now</a>
        </div>
        <div class="hero-img">
          <img src="https://picsum.photos/seed/livingroom/700/500" alt="Cozy modern living room" loading="lazy">
        </div>
      </div>
    </section>
 
    <!-- FEATURES STRIP -->
    <section class="features">
      <div class="container feature-row">
        <div class="feature"><span>🚚</span><h4>Free Delivery</h4><p>On orders above ₹2,999</p></div>
        <div class="feature"><span>🔄</span><h4>Easy Returns</h4><p>30-day return policy</p></div>
        <div class="feature"><span>🔒</span><h4>Secure Payment</h4><p>UPI, cards &amp; net banking</p></div>
        <div class="feature"><span>💬</span><h4>24/7 Support</h4><p>We're always here to help</p></div>
      </div>
    </section>
 
    <!-- PRODUCTS / SERVICES -->
    <section id="products" class="section">
      <div class="container">
        <h2 class="section-title">Our Products</h2>
        <div class="card-row">
          <article class="card">
            <img src="https://picsum.photos/seed/sofa/400/300" alt="Modern sofa" loading="lazy">
            <div class="card-body">
              <h3>Nordic Sofa</h3>
              <p>Three-seater with soft fabric upholstery.</p>
              <div class="card-foot"><span class="price">₹24,999</span><a href="#" class="btn btn-small">Add to Cart</a></div>
            </div>
          </article>
          <article class="card">
            <img src="https://picsum.photos/seed/lamp/400/300" alt="Table lamp" loading="lazy">
            <div class="card-body">
              <h3>Arc Table Lamp</h3>
              <p>Warm LED lighting with a brass finish.</p>
              <div class="card-foot"><span class="price">₹3,499</span><a href="#" class="btn btn-small">Add to Cart</a></div>
            </div>
          </article>
          <article class="card">
            <img src="https://picsum.photos/seed/chair/400/300" alt="Wooden chair" loading="lazy">
            <div class="card-body">
              <h3>Oak Dining Chair</h3>
              <p>Solid oak frame with ergonomic back support.</p>
              <div class="card-foot"><span class="price">₹5,799</span><a href="#" class="btn btn-small">Add to Cart</a></div>
            </div>
          </article>
          <article class="card">
            <img src="https://picsum.photos/seed/decor/400/300" alt="Home decor" loading="lazy">
            <div class="card-body">
              <h3>Decor Set</h3>
              <p>Vases, frames and wall art to finish any room.</p>
              <div class="card-foot"><span class="price">₹1,999</span><a href="#" class="btn btn-small">Add to Cart</a></div>
            </div>
          </article>
        </div>
      </div>
    </section>
 
    <!-- ABOUT US -->
    <section id="about" class="section alt">
      <div class="container about-row">
        <div class="about-img">
          <img src="https://picsum.photos/seed/studio/600/450" alt="Our design studio" loading="lazy">
        </div>
        <div class="about-text">
          <h2 class="section-title left">About Us</h2>
          <p>Founded in 2018 in Chennai, UrbanNest began with a simple idea: good design should be affordable. Our team of designers works directly with artisans to create durable, beautiful pieces for modern homes.</p>
          <ul class="stats">
            <li><strong>50K+</strong> Happy customers</li>
            <li><strong>500+</strong> Products</li>
            <li><strong>25</strong> Cities served</li>
          </ul>
        </div>
      </div>
    </section>
 
    <!-- CONTACT DETAILS -->
    <section id="contact" class="section">
      <div class="container">
        <h2 class="section-title">Contact Us</h2>
        <div class="contact-row">
          <div class="contact-info">
            <h3>Get in Touch</h3>
            <p>📍 No.123,saveetha nagar,chennai - 602013</p>
            <p>📞 +91 8939902735</p>
            <p>✉️ support@saveetha.com</p>
            <p>🕘 Mon – Sat, 9:00 AM – 7:00 PM</p>
          </div>
          <form class="contact-form" onsubmit="event.preventDefault(); alert('Thanks! We will get back to you soon.'); this.reset();">
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea rows="4" placeholder="Your Message" required></textarea>
            <button type="submit" class="btn">Send Message</button>
          </form>
        </div>
      </div>
    </section>
 
    <!-- USER ACCOUNT -->
    <section id="account" class="section alt">
      <div class="container">
        <h2 class="section-title">User Account</h2>
        <div class="account-row">
          <form class="account-box" onsubmit="event.preventDefault(); alert('Login successful (demo).');">
            <h3>Login</h3>
            <input type="email" placeholder="Email" required>
            <input type="password" placeholder="Password" required>
            <button type="submit" class="btn">Login</button>
          </form>
          <form class="account-box" onsubmit="event.preventDefault(); alert('Account created (demo).'); this.reset();">
            <h3>Create Account</h3>
            <input type="text" placeholder="Full Name" required>
            <input type="email" placeholder="Email" required>
            <input type="password" placeholder="Password" required>
            <button type="submit" class="btn">Sign Up</button>
          </form>
        </div>
      </div>
    </section>
  </main>
 
  <!-- FOOTER -->
  <footer class="site-footer">
    <div class="container footer-inner">
      <div class="social">
        <a href="https://facebook.com" target="_blank" rel="noopener">Facebook</a>
        <a href="https://instagram.com" target="_blank" rel="noopener">Instagram</a>
        <a href="https://twitter.com" target="_blank" rel="noopener">Twitter</a>
        <a href="https://linkedin.com" target="_blank" rel="noopener">LinkedIn</a>
        <a href="https://youtube.com" target="_blank" rel="noopener">YouTube</a>
      </div>
      <p>&copy; 2026 UrbanNest. All rights reserved.</p>
    </div>
  </footer>
 
</body>
</html>
```
### CSS
```css
/* ========== GLOBAL STYLES ========== */
:root {
  --primary: #c8553d;
  --primary-dark: #a64430;
  --dark: #2b2d42;
  --light: #f8f5f2;
  --white: #ffffff;
  --grey: #6c6f7d;
}
 
* { margin: 0; padding: 0; box-sizing: border-box; }
html { scroll-behavior: smooth; }
 
body {
  font-family: 'Segoe UI', Roboto, Arial, sans-serif;
  color: var(--dark);
  line-height: 1.6;
  background: var(--white);
}
 
img { max-width: 100%; display: block; }
a { text-decoration: none; color: inherit; }
ul { list-style: none; }
 
.container { width: 90%; max-width: 1150px; margin: 0 auto; }
.section { padding: 70px 0; }
.alt { background: var(--light); }
 
.section-title { text-align: center; font-size: 2rem; margin-bottom: 40px; position: relative; }
.section-title::after {
  content: ""; display: block; width: 60px; height: 4px;
  background: var(--primary); margin: 10px auto 0; border-radius: 2px;
}
.section-title.left { text-align: left; }
.section-title.left::after { margin-left: 0; }
 
/* ========== BUTTONS ========== */
.btn {
  display: inline-block; background: var(--primary); color: var(--white);
  padding: 12px 28px; border: none; border-radius: 30px; cursor: pointer;
  font-size: 1rem; font-weight: 600;
  transition: background 0.3s ease, transform 0.3s ease, box-shadow 0.3s ease;
}
.btn:hover { background: var(--primary-dark); transform: translateY(-3px); box-shadow: 0 8px 18px rgba(200, 85, 61, 0.35); }
.btn-small { padding: 8px 18px; font-size: 0.9rem; }
 
/* ========== HEADER & NAVBAR (Flexbox) ========== */
.site-header { background: var(--white); position: sticky; top: 0; z-index: 100; box-shadow: 0 2px 10px rgba(0,0,0,0.08); }
.nav-wrap { display: flex; justify-content: space-between; align-items: center; padding: 16px 0; flex-wrap: wrap; gap: 10px; }
.logo { font-size: 1.7rem; font-weight: 800; }
.logo span { color: var(--primary); }
.nav-links { display: flex; align-items: center; gap: 28px; flex-wrap: wrap; }
.nav-links a:not(.btn) { font-weight: 500; position: relative; transition: color 0.3s; }
.nav-links a:not(.btn)::after {
  content: ""; position: absolute; left: 0; bottom: -4px; width: 0; height: 2px;
  background: var(--primary); transition: width 0.3s ease;
}
.nav-links a:not(.btn):hover { color: var(--primary); }
.nav-links a:not(.btn):hover::after { width: 100%; }
 
/* ========== HERO (Flexbox) ========== */
.hero { background: linear-gradient(135deg, #fdf0ec, #f8f5f2); padding: 80px 0; }
.hero-inner { display: flex; align-items: center; justify-content: space-between; gap: 50px; flex-wrap: wrap; }
.hero-text { flex: 1 1 380px; }
.eyebrow { color: var(--primary); font-weight: 700; text-transform: uppercase; letter-spacing: 2px; font-size: 0.85rem; }
.hero-text h1 { font-size: 3rem; line-height: 1.2; margin: 12px 0 18px; }
.hero-text p { color: var(--grey); margin-bottom: 26px; }
.hero-img { flex: 1 1 380px; }
.hero-img img { border-radius: 20px; box-shadow: 0 20px 40px rgba(0,0,0,0.15); transition: transform 0.5s ease; }
.hero-img img:hover { transform: scale(1.03); }
 
/* ========== FEATURES STRIP ========== */
.features { background: var(--dark); color: var(--white); padding: 30px 0; }
.feature-row { display: flex; justify-content: space-between; flex-wrap: wrap; gap: 20px; }
.feature { flex: 1 1 200px; text-align: center; }
.feature span { font-size: 1.8rem; }
.feature h4 { margin: 4px 0 2px; }
.feature p { font-size: 0.9rem; opacity: 0.75; }
 
/* ========== PRODUCT CARDS (Flexbox) ========== */
.card-row { display: flex; flex-wrap: wrap; gap: 24px; justify-content: center; }
.card {
  flex: 1 1 240px; max-width: 270px; background: var(--white); border-radius: 14px;
  overflow: hidden; box-shadow: 0 4px 14px rgba(0,0,0,0.08);
  display: flex; flex-direction: column;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.card:hover { transform: translateY(-8px); box-shadow: 0 14px 30px rgba(0,0,0,0.16); }
.card img { width: 100%; height: 180px; object-fit: cover; transition: transform 0.4s ease; }
.card:hover img { transform: scale(1.08); }
.card { overflow: hidden; }
.card-body { padding: 18px; display: flex; flex-direction: column; flex: 1; }
.card-body h3 { margin-bottom: 6px; }
.card-body p { color: var(--grey); font-size: 0.92rem; flex: 1; }
.card-foot { display: flex; justify-content: space-between; align-items: center; margin-top: 16px; }
.price { font-weight: 800; font-size: 1.1rem; color: var(--primary); }
 
/* ========== ABOUT (Flexbox) ========== */
.about-row { display: flex; align-items: center; gap: 50px; flex-wrap: wrap; }
.about-img { flex: 1 1 340px; }
.about-img img { border-radius: 16px; box-shadow: 0 12px 28px rgba(0,0,0,0.12); }
.about-text { flex: 1 1 340px; }
.about-text p { color: var(--grey); margin-bottom: 24px; }
.stats { display: flex; gap: 30px; flex-wrap: wrap; }
.stats li { display: flex; flex-direction: column; color: var(--grey); font-size: 0.9rem; }
.stats strong { font-size: 1.8rem; color: var(--primary); }
 
/* ========== CONTACT (Flexbox) ========== */
.contact-row { display: flex; gap: 40px; flex-wrap: wrap; }
.contact-info { flex: 1 1 300px; background: var(--dark); color: var(--white); padding: 32px; border-radius: 14px; }
.contact-info h3 { margin-bottom: 16px; }
.contact-info p { margin-bottom: 12px; opacity: 0.9; }
.contact-form { flex: 1 1 340px; display: flex; flex-direction: column; gap: 14px; }
 
input, textarea {
  width: 100%; padding: 13px 16px; border: 2px solid #e2dfdc; border-radius: 10px;
  font-family: inherit; font-size: 1rem; outline: none; background: var(--white);
  transition: border-color 0.3s, box-shadow 0.3s;
}
input:focus, textarea:focus { border-color: var(--primary); box-shadow: 0 0 0 4px rgba(200,85,61,0.12); }
.contact-form .btn { align-self: flex-start; }
 
/* ========== USER ACCOUNT (Flexbox) ========== */
.account-row { display: flex; justify-content: center; gap: 30px; flex-wrap: wrap; }
.account-box {
  flex: 1 1 300px; max-width: 420px; background: var(--white); padding: 30px;
  border-radius: 14px; box-shadow: 0 4px 14px rgba(0,0,0,0.08);
  display: flex; flex-direction: column; gap: 14px;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.account-box:hover { transform: translateY(-5px); box-shadow: 0 12px 26px rgba(0,0,0,0.14); }
.account-box .btn { align-self: flex-start; }
 
/* ========== FOOTER (Flexbox) ========== */
.site-footer { background: var(--dark); color: var(--white); padding: 28px 0; }
.footer-inner { display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 14px; }
.social { display: flex; gap: 20px; flex-wrap: wrap; }
.social a { opacity: 0.8; transition: color 0.3s, opacity 0.3s, transform 0.3s; display: inline-block; }
.social a:hover { color: var(--primary); opacity: 1; transform: translateY(-3px); }
.site-footer p { font-size: 0.9rem; opacity: 0.7; }
 
/* ========== RESPONSIVE ========== */
@media (max-width: 768px) {
  .nav-wrap { flex-direction: column; }
  .nav-links { justify-content: center; gap: 16px; }
  .hero-text h1 { font-size: 2.2rem; }
  .hero { padding: 50px 0; }
  .footer-inner { flex-direction: column; text-align: center; }
  .social { justify-content: center; }
}
```
## OUTPUT
<img width="1917" height="1090" alt="image" src="https://github.com/user-attachments/assets/5108a84a-2b1f-4652-a133-06f35ba073b3" />

<img width="1917" height="1091" alt="image" src="https://github.com/user-attachments/assets/32caeb66-b470-4f57-abc7-4d61e8fcc092" />

<img width="1916" height="1147" alt="image" src="https://github.com/user-attachments/assets/342b6549-3067-453b-aff2-7ae4122d57c6" />

<img width="1917" height="1108" alt="image" src="https://github.com/user-attachments/assets/bf4b9981-128f-47ce-b2c0-f1c1309aa800" />

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
