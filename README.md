# The-Roof-Restaurant-Lakhisarai-
“Restaurant website project”
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Roof Restaurant - Rooftop Dining in Lakhisarai</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Poppins', sans-serif; line-height: 1.6; color: #fff; background: #000; overflow-x: hidden; }

        /* Navigation */
        nav { position: fixed; top: 0; width: 100%; background: rgba(0,0,0,0.95); backdrop-filter: blur(10px); z-index: 1000; padding: 1rem 0; }
        .nav-container { max-width: 1200px; margin: 0 auto; display: flex; justify-content: space-between; align-items: center; padding: 0 2rem; }
        .logo { font-size: 1.8rem; font-weight: 700; color: #FFD700; text-decoration: none; }
        .nav-links { display: flex; list-style: none; gap: 2rem; }
        .nav-links a { color: #fff; text-decoration: none; font-weight: 500; transition: color 0.3s ease; }
        .nav-links a:hover { color: #FFD700; }

        /* Hero Section */
        .hero { height: 100vh; background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('https://images.unsplash.com/photo-1533777324565-a040eb52facd?auto=format&fit=crop&q=80&w=2000'); background-size: cover; background-position: center; display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center; }
        .hero h1 { font-size: 4rem; color: #FFD700; margin-bottom: 1rem; }
        .hero p { font-size: 1.5rem; margin-bottom: 2rem; }

        /* Buttons */
        .btn { padding: 1rem 2rem; border-radius: 50px; text-decoration: none; font-weight: 600; transition: 0.3s; display: inline-flex; align-items: center; gap: 0.5rem; }
        .btn-primary { background: #FFD700; color: #000; }
        .btn-secondary { border: 2px solid #FFD700; color: #fff; margin-left: 10px; }
        .btn:hover { transform: translateY(-3px); opacity: 0.9; }

        /* Menu & Features */
        section { padding: 5rem 2rem; max-width: 1200px; margin: 0 auto; }
        .section-title { font-size: 3rem; text-align: center; margin-bottom: 3rem; color: #FFD700; }
        .menu-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2rem; }
        .menu-category { background: rgba(255,255,255,0.05); padding: 2rem; border-radius: 20px; }
        .menu-item { display: flex; justify-content: space-between; padding: 0.8rem 0; border-bottom: 1px solid rgba(255,255,255,0.1); }

        /* Contact & Map */
        .contact-info { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2rem; margin-bottom: 2rem; }
        .contact-item { padding: 2rem; background: rgba(255,255,255,0.05); border-radius: 20px; text-align: center; }
        #map { width: 100%; height: 400px; border-radius: 20px; border: none; }

        /* Floating WhatsApp */
        .whatsapp-float { position: fixed; bottom: 40px; right: 40px; background: #25d366; color: #fff; width: 60px; height: 60px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 30px; z-index: 100; transition: 0.3s; }
        .whatsapp-float:hover { transform: scale(1.1); }

        @media (max-width: 768px) {
            .nav-links { display: none; }
            .hero h1 { font-size: 2.5rem; }
        }
    </style>
</head>
<body>

    <nav>
        <div class="nav-container">
            <a href="#" class="logo">The Roof Restaurant</a>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#menu">Menu</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </nav>

    <section id="home" class="hero">
        <h1>The Roof Restaurant</h1>
        <p>Experience Rooftop Dining in Lakhisarai</p>
        <div>
            <a href="#menu" class="btn btn-primary"><i class="fas fa-utensils"></i> View Menu</a>
            <a href="tel:+918252225708" class="btn btn-secondary"><i class="fas fa-phone"></i> Call Now</a>
        </div>
    </section>

    <section id="menu">
        <h2 class="section-title">Our Menu</h2>
        <div class="menu-grid">
            <div class="menu-category">
                <h3><i class="fas fa-seedling"></i> Veg Starters</h3>
                <div class="menu-item"><span>Paneer Chilli</span><span>₹180</span></div>
                <div class="menu-item"><span>Veg Manchurian</span><span>₹150</span></div>
            </div>
            <div class="menu-category">
                <h3><i class="fas fa-drumstick-bite"></i> Non-Veg</h3>
                <div class="menu-item"><span>Chicken Lollipop</span><span>₹220</span></div>
                <div class="menu-item"><span>Tandoori Chicken</span><span>₹280</span></div>
            </div>
        </div>
    </section>

    <section id="contact">
        <h2 class="section-title">Visit Us</h2>
        <div class="contact-info">
            <div class="contact-item">
                <i class="fas fa-map-marker-alt" style="font-size: 2rem; color: #FFD700;"></i>
                <p>Purani Bazaar, Lakhisarai, Bihar</p>
            </div>
            <div class="contact-item">
                <i class="fas fa-phone" style="font-size: 2rem; color: #FFD700;"></i>
                <p>+91 8252225708</p>
            </div>
        </div>
        <iframe id="map" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3612.4431713364413!2d86.0911!3d25.1748!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zMjXCsDEwJzI5LjMiTiA4NsKwMDUnMjguMCJF!5e0!3m2!1sen!2sin!4v1650000000000"></iframe>
    </section>

    <footer style="text-align: center; padding: 2rem; border-top: 1px solid #333;">
        <p>© 2026 The Roof Restaurant. All rights reserved.</p>
    </footer>

    <a href="https://wa.me/918252225708" class="whatsapp-float" target="_blank">
        <i class="fab fa-whatsapp"></i>
    </a>

</body>
</html>
