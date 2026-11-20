<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SparkleClean Services</title>
    <style>
        /* Reset & Base Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            line-height: 1.6;
            color: #333;
        }

        /* Navigation */
        header {
            background: #ffffff;
            padding: 1rem 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: #0284c7;
        }

        nav a {
            text-decoration: none;
            color: #333;
            margin-left: 20px;
            font-weight: 500;
        }

        nav a:hover {
            color: #0284c7;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(2, 132, 199, 0.85), rgba(2, 132, 199, 0.85)), 
                        url('https://unsplash.com') center/cover;
            color: white;
            text-align: center;
            padding: 100px 20px;
        }

        .hero h1 {
            font-size: 2.8rem;
            margin-bottom: 1rem;
        }

        .hero p {
            font-size: 1.2rem;
            max-width: 600px;
            margin: 0 auto 2rem auto;
        }

        .btn {
            display: inline-block;
            background: #f59e0b;
            color: white;
            padding: 12px 30px;
            text-decoration: none;
            border-radius: 5px;
            font-weight: bold;
            transition: background 0.3s;
            border: none;
            cursor: pointer;
            font-size: 1rem;
        }

        .btn:hover {
            background: #d97706;
        }

        /* Services Section */
        .services {
            padding: 60px 5%;
            text-align: center;
            background: #f8fafc;
        }

        .services h2 {
            font-size: 2rem;
            margin-bottom: 40px;
            color: #0f172a;
        }

        .service-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
            max-width: 1100px;
            margin: 0 auto;
        }

        .card {
            background: white;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            transition: transform 0.2s;
        }

        .card:hover {
            transform: translateY(-5px);
        }

        .card h3 {
            color: #0284c7;
            margin-bottom: 15px;
        }

        /* Contact / Quote Section */
        .contact {
            padding: 60px 5%;
            max-width: 600px;
            margin: 0 auto;
            text-align: center;
        }

        .contact h2 {
            margin-bottom: 20px;
            color: #0f172a;
        }

        form {
            display: flex;
            flex-direction: column;
            gap: 15px;
            text-align: left;
        }

        input, select, textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #cbd5e1;
            border-radius: 5px;
            font-size: 1rem;
        }

        /* Footer */
        footer {
            background: #0f172a;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 40px;
        }

        /* Mobile Adjustments */
        @media (max-width: 600px) {
            .hero h1 { font-size: 2rem; }
            nav { display: none; } /* Hides nav links on very small screens for simplicity */
        }
    </style>
</head>
<body>

    <!-- Header -->
    <header>
        <div class="logo">SparkleClean</div>
        <nav>
            <a href="#home">Home</a>
            <a href="#services">Services</a>
            <a href="#quote">Get a Quote</a>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <h1>A Spotless Home, Without the Hassle</h1>
        <p>Reliable, eco-friendly residential and commercial cleaning tailored to your schedule.</p>
        <a href="#quote" class="btn">Book a Cleaning</a>
    </section>

    <!-- Services Section -->
    <section class="services" id="services">
        <h2>Our Cleaning Services</h2>
        <div class="service-grid">
            <div class="card">
                <h3>Standard Home Cleaning</h3>
                <p>Routine dusting, vacuuming, mopping, and bathroom sanitization to keep your home fresh.</p>
            </div>
            <div class="card">
                <h3>Deep Cleaning</h3>
                <p>Top-to-bottom intensive scrubbing, including baseboards, inside appliances, and hard-to-reach areas.</p>
            </div>
            <div class="card">
                <h3>Office & Commercial</h3>
                <p>After-hours workspace sanitization to keep your employees healthy and productive.</p>
            </div>
        </div>
    </section>

    <!-- Quote Form Section -->
    <section class="contact" id="quote">
        <h2>Request a Free Quote</h2>
        <form>
            <input type="text" placeholder="Your Full Name" required>
            <input type="email" placeholder="Email Address" required>
            <input type="tel" placeholder="Phone Number" required>
            <select required>
                <option value="">Select Service Type...</option>
                <option value="standard">Standard Home Cleaning</option>
                <option value="deep">Deep Cleaning</option>
                <option value="commercial">Office / Commercial</option>
            </select>
            <textarea rows="4" placeholder="Tell us about your space (e.g., number of bedrooms/bathrooms)"></textarea>
            <button type="submit" class="btn">Submit Request</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 SparkleClean Services. All rights reserved.</p>
    </footer>

</body>
</html>
