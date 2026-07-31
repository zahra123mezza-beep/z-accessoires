<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Z Accessories</title>
    <style>
        /* Importing elegant fonts for the design */
        @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,600;1,400&family=Lato:wght@300;400&display=swap');

        :root {
            --bg-color: #f4efeb;
            --text-color: #5c4331;
            --accent-color: #d8b8a8;
        }

        body {
            margin: 0;
            padding: 0;
            font-family: 'Lato', sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 1.8;
            overflow-x: hidden;
        }

        h1, h2, h3 {
            font-family: 'Playfair Display', serif;
            font-weight: 400;
            margin: 0 0 20px 0;
        }

        /* Hero Section (Image 1) */
        .hero {
            position: relative;
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            /* Applying Image 1 as the background */
            background-image: url('@_z.accessories_ - 1.png');
            background-size: cover;
            background-position: center;
            color: var(--text-color);
            padding: 20px;
        }

        /* Adding a slight overlay so text is readable if the image is busy */
        .hero::before {
            content: '';
            position: absolute;
            top: 0; left: 0; right: 0; bottom: 0;
            background: rgba(244, 239, 235, 0.4);
            z-index: 1;
        }

        .hero-content {
            position: relative;
            z-index: 2;
        }

        .hero h1 {
            font-size: 2.5rem;
            letter-spacing: 2px;
            text-transform: uppercase;
            margin-bottom: 10px;
        }

        .hero p {
            font-family: 'Playfair Display', serif;
            font-size: 3.5rem;
            font-style: italic;
            margin-bottom: 40px;
        }

        .btn {
            display: inline-block;
            padding: 15px 30px;
            background-color: transparent;
            color: var(--text-color);
            border: 1px solid var(--text-color);
            text-decoration: none;
            font-family: 'Lato', sans-serif;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: all 0.3s ease;
        }

        .btn:hover {
            background-color: var(--text-color);
            color: var(--bg-color);
        }

        /* Standard Section Layout */
        section {
            padding: 100px 10%;
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            justify-content: space-between;
            gap: 60px;
        }

        section.reverse {
            flex-direction: row-reverse;
        }

        .content-block {
            flex: 1;
            min-width: 300px;
        }

        .image-block {
            flex: 1;
            min-width: 300px;
        }

        .image-block img {
            width: 100%;
            height: auto;
            object-fit: cover;
            box-shadow: 0 10px 30px rgba(92, 67, 49, 0.1);
        }

        .section-title {
            font-size: 5rem;
            margin-bottom: 10px;
            letter-spacing: -2px;
        }

        .sub-title {
            font-size: 3rem;
            margin-bottom: 20px;
        }
        
        .content-block ul {
            list-style-type: none;
            padding: 0;
            font-size: 1.2rem;
        }

        .content-block ul li {
            margin-bottom: 15px;
            padding-left: 20px;
            position: relative;
        }

        .content-block ul li::before {
            content: "—";
            position: absolute;
            left: 0;
            color: var(--accent-color);
        }

        /* Footer Layout (Image 5 aesthetic) */
        footer {
            text-align: center;
            padding: 80px 20px;
            background-color: var(--bg-color);
            border-top: 1px solid rgba(92, 67, 49, 0.2);
            position: relative;
        }

        footer h2 {
            font-size: 6rem;
            margin-bottom: 20px;
        }

        footer p {
            font-size: 1.2rem;
            margin: 10px 0;
        }

        .social-handle {
            display: block;
            margin-top: 30px;
            font-weight: 400;
            letter-spacing: 2px;
            font-size: 1.1rem;
        }

        /* Responsive Design for Mobile */
        @media (max-width: 768px) {
            .hero h1 { font-size: 1.8rem; }
            .hero p { font-size: 2.5rem; }
            .section-title { font-size: 3.5rem; }
            .sub-title { font-size: 2rem; }
            footer h2 { font-size: 4rem; }
            section { padding: 60px 5%; }
        }
    </style>
</head>
<body>

    <!-- Hero Section using Image 1 -->
    <div class="hero">
        <div class="hero-content">
            <h1>Got a vision? Or need something ready?</h1>
            <p>Pearls, Crystals & Charms</p>
            <a href="#contact" class="btn">DM to order or customize</a>
        </div>
    </div>

    <!-- Ready-To-Wear Section using Image 2 -->
    <section id="ready-to-wear">
        <div class="image-block">
            <img src="@_z.accessories_ - 2.png" alt="Ready to wear collection">
        </div>
        <div class="content-block">
            <h2 class="section-title">Shop Ready-To-Wear</h2>
            <h3 class="sub-title">Limited Edition</h3>
            <p>Grab our pre-designed, limited-edition accessories directly from the shop at super friendly prices! Each piece is crafted with pearls, crystals, and charms for a one-of-a-kind look.</p>
            <br>
            <p>Pre-designed & ready to ship. Exclusive drops at prices you'll love — shop before they're gone!</p>
        </div>
    </section>

    <!-- Custom Design Section using Image 3 -->
    <section id="custom" class="reverse">
        <div class="image-block">
            <img src="@_z.accessories_ - 3.png" alt="Custom design pieces">
        </div>
        <div class="content-block">
            <h2 class="section-title">custom</h2>
            <h3 class="sub-title">Custom Design</h3>
            <p>Provide your item and we'll hand-embellish it with pearls, crystals, or charms — fully custom to your request. Every piece is one-of-a-kind, made just for you.</p>
        </div>
    </section>

    <!-- Contact Section using Image 4 -->
    <section id="contact">
        <div class="image-block">
            <img src="@_z.accessories_ - 4.png" alt="Model showing custom embellished bag">
        </div>
        <div class="content-block">
            <h2 class="section-title">reach out</h2>
            <h3 class="sub-title">Let's Create Together</h3>
            <ul>
                <li>Slide into our DMs</li>
                <li>Claim a ready-to-wear piece</li>
                <li>Or start your custom design</li>
            </ul>
        </div>
    </section>

    <!-- Footer based on Image 5 -->
    <footer>
        <h2>Thank You</h2>
        <p>for being here & supporting our craft!</p>
        <p>We can't wait to add a little extra sparkle to your day.</p>
        <p>DM us to get started</p>
        <span class="social-handle">@_z.accessories_</span>
    </footer>

</body>
</html>
