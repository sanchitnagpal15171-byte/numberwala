<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>  | Fancy Car Numbers</title>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&display=swap" rel="stylesheet">
<style>
  /* Global Styles */
  * {margin: 0; padding: 0; box-sizing: border-box;}
  body {font-family: 'Montserrat', sans-serif; color: #1a1a1a; background-color: #f8f8f8; line-height: 1.6;}
  a {text-decoration: none; color: inherit;}
  img {max-width: 100%; display: block;}

  /* Header */
  header {display: flex; justify-content: space-between; align-items: center; padding: 20px 50px; background: #111;}
  header .logo {font-size: 1.8rem; font-weight: 700; color: #fff;}
  nav ul {list-style: none; display: flex; gap: 25px;}
  nav ul li a {color: White; font-weight: 500; transition: 0.3s;}
  nav ul li a:hover {color: #ffcd00;}

  /* Hero Section */
  .hero {display: flex; align-items: center; justify-content: space-between; padding: 80px 50px; background: url('https://images.unsplash.com/photo-1563720221162-cd460fc6f26e') center/cover no-repeat; color: orange;}
  .hero-text {max-width: 600px;}
  .hero-text h1 {font-size: 3rem; margin-bottom: 20px;}
  .hero-text p {font-size: 1.2rem; margin-bottom: 30px;}
  .hero-text a {background: #ffcd00; color: #111; padding: 15px 30px; font-weight: 600; border-radius: 5px; transition: 0.3s;}
  .hero-text a:hover {background: #e6b800;}

  /* Services */
  .services {padding: 80px 50px; background: #fff; text-align: center;}
  .services h2 {font-size: 2.5rem; margin-bottom: 50px;}
  .service-card {display: inline-block; width: 300px; background: #f4f4f4; margin: 15px; border-radius: 10px; padding: 30px; transition: 0.3s;}
  .service-card:hover {transform: translateY(-10px);}
  .service-card h3 {margin-bottom: 15px; color: #111;}
  .service-card p {color: #555;}

  /* Gallery */
  .gallery {padding: 80px 50px; background: #f0f0f0; text-align: center;}
  .gallery h2 {font-size: 2.5rem; margin-bottom: 50px;}
  .gallery-grid {display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px;}
  .gallery-grid img {border-radius: 10px; transition: 0.3s;}
  .gallery-grid img:hover {transform: scale(1.05);}

  /* Pricing */
  .pricing {padding: 80px 50px; text-align: center; background: #fff;}
  .pricing h2 {font-size: 2.5rem; margin-bottom: 50px;}
  .pricing-cards {display: flex; flex-wrap: wrap; justify-content: center; gap: 30px;}
  .pricing-card {background: #f4f4f4; padding: 40px; border-radius: 15px; width: 300px; transition: 0.3s;}
  .pricing-card:hover {transform: translateY(-10px);}
  .pricing-card h3 {margin-bottom: 15px;}
  .pricing-card p {margin-bottom: 25px; color: #555;}
  .pricing-card span {display: block; font-size: 1.8rem; font-weight: 700; margin-bottom: 20px;}
  .pricing-card a {background: #ffcd00; color: #111; padding: 12px 25px; border-radius: 5px; font-weight: 600;}

  /* Testimonials */
  .testimonials {padding: 80px 50px; background: #f0f0f0; text-align: center;}
  .testimonials h2 {font-size: 2.5rem; margin-bottom: 50px;}
  .testimonial-card {background: #fff; padding: 30px; border-radius: 10px; display: inline-block; max-width: 300px; margin: 15px; transition: 0.3s;}
  .testimonial-card:hover {transform: translateY(-10px);}
  .testimonial-card p {margin-bottom: 15px; color: #555;}
  .testimonial-card h4 {font-weight: 600; color: #111;}

  /* Contact */
  .contact {padding: 80px 50px; background: #111; color: Blue; text-align: center;}
  .contact h2 {font-size: 2.5rem; margin-bottom: 30px;}
  .contact form {max-width: 500px; margin: 0 auto;}
  .contact input, .contact textarea {width: 100%; padding: 15px; margin-bottom: 20px; border-radius: 5px; border: none;}
  .contact button {background: #ffcd00; color: Black; padding: 15px 30px; font-weight: 600; border-radius: 5px; transition: 0.3s;}
  .contact button:hover {background: #e6b800;}

  /* Footer */
  footer {padding: 20px 50px; background: #111; color: Black; text-align: center;}
  footer p {font-size: 0.9rem;}
  
  @media (max-width: 768px) {
    header {flex-direction: column; gap: 15px;}
    .hero {flex-direction: column; text-align: center; gap: 30px;}
    .pricing-cards {flex-direction: column; align-items: center;}
  }
</style>
</head>
<body>

<!-- Header -->
<header>
  <div class="logo">numberwala_</div>
  <nav>
    <ul>
      <li><a href="#services">Services</a></li>
      <li><a href="#gallery">Gallery</a></li>
      <li><a href="#pricing">Pricing</a></li>
      <li><<a href="tel:+919876543210">
  <button>Contact Us</button>
</a></li>
    </ul>
  </nav>
</header>

<!-- Hero Section -->
<section class="hero">
  <div class="hero-text">
    <h1>Drive Your Status. Own the Plate.</h1>
    <p>Premium, unique, and memorable car numbers for those who demand the best.</p>
    <a href="#contact">Book Your Plate</a>
  </div>
</section>

<!-- Services Section -->
<section id="services" class="services">
  <h2>Our Exclusive Services</h2>
  <div class="service-card">
    <h3>Luxury Number Plates</h3>
    <p>Exclusive, one-of-a-kind number plates that turn heads wherever you go.</p>
  </div>
  <div class="service-card">
    <h3>Custom Designs</h3>
    <p>Create a unique plate that matches your personality and style.</p>
  </div>
  <div class="service-card">
    <h3>VIP Consultation</h3>
    <p>Expert advice to secure the most prestigious numbers available.</p>
  </div>
</section>

<!-- Gallery Section -->
<section id="gallery" class="gallery">
  <h2>Gallery of Elite Plates</h2>
  <div class="gallery-grid">
    <img src="https://images.unsplash.com/photo-1612874749256-6c08e4b6a41f" alt="Fancy Number Plate 1">
    <img src="https://images.unsplash.com/photo-1597009112547-3c7b6a8b0320" alt="Fancy Number Plate 2">
    <img src="https://images.unsplash.com/photo-1612874749288-8bde02c8f2f4" alt="Fancy Number Plate 3">
    <img src="https://images.unsplash.com/photo-1605902711622-cfb43c4433c5" alt="Fancy Number Plate 4">
  </div>
</section>

<!-- Pricing Section -->
<section id="pricing" class="pricing">
  <h2>Our Packages</h2>
  <div class="pricing-cards">
    <div class="pricing-card">
      <h3>Silver</h3>
      <span>Rs.115000/-</span>
      <p>Standard numbers with elegant design options.</p>
      <a href="#contact">Choose Plan</a>
    </div>
    <div class="pricing-card">
      <h3>Gold</h3>
      <span>Rs.350000/-</span>
      <p>Premium numbers with exclusive customization.</p>
      <a href="#contact">Choose Plan</a>
    </div>
    <div class="pricing-card">
      <h3>Platinum</h3>
      <span>Rs.600000/-</span>
      <p>Ultra-exclusive VIP numbers with personal consultation.</p>
      <a href="#contact">Choose Plan</a>
    </div>
  </div>
</section>

<!-- Testimonials Section -->
<section class="testimonials">
  <h2>What Our Clients Say</h2>
  <div class="testimonial-card">
    <p>"Elite Plates transformed my car’s presence. Truly exceptional service!"</p>
    <h4>- John D.</h4>
  </div>
  <div class="testimonial-card">
    <p>"The number plate design was unique and worth every penny. Highly recommend!"</p>
    <h4>- Sarah K.</h4>
  </div>
</section>

<!-- Contact Section -->
<section id="contact" class="contact">
  <h2>Book Your Fancy Number Plate</h2>
  <form>
    <input type="text" placeholder="Full Name" required>
    <input type="email" placeholder="Email Address" required>
    <input type="tel" placeholder="Phone Number" required>
    <textarea rows="5" placeholder="Message / Requirements"></textarea>
    <button type="submit">Submit Request</button>
  </form>
</section>

<!-- Footer -->
<footer>
  <p>&copy; 2026 numberwala_. All Rights Reserved.</p>
</footer>

</body>
</html>
