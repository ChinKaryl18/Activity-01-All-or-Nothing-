
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Technology Showcase</title>

    <style>
        /* GENERAL STYLE */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, sans-serif;
            background: #080d1a;
            color: white;
            line-height: 1.6;
        }

        /* NAVIGATION BAR */
        header {
            background: #101a30;
            padding: 20px 8%;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 25px;
            font-weight: bold;
            letter-spacing: 2px;
        }

        .logo span {
            color: #00d9ff;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 25px;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            transition: 0.3s;
        }

        .nav-links a:hover {
            color: #00d9ff;
        }

        /* HERO SECTION */
        .hero {
            min-height: 90vh;
            display: flex;
            align-items: center;
            padding: 60px 10%;
            background:
                linear-gradient(
                    rgba(5,10,25,0.65),
                    rgba(5,10,25,0.85)
                ),
                url("https://images.unsplash.com/photo-1451187580459-43490279c0fa?w=1600")
                center/cover no-repeat;
        }

        .hero-content {
            max-width: 650px;
        }

        .hero h1 {
            font-size: 65px;
            line-height: 1.2;
            margin-bottom: 20px;
        }

        .hero h1 span {
            color: #00d9ff;
        }

        .hero p {
            font-size: 18px;
            color: #d0d9e8;
            margin-bottom: 30px;
        }

        .btn {
            display: inline-block;
            background: #00bfe9;
            color: #08101e;
            padding: 13px 28px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
            transition: 0.3s;
        }

        .btn:hover {
            background: white;
            transform: translateY(-4px);
        }

        /* SECTION DESIGN */
        .section {
            padding: 80px 8%;
        }

        .section-title {
            text-align: center;
            font-size: 36px;
            color: #00d9ff;
            margin-bottom: 10px;
        }

        .subtitle {
            text-align: center;
            color: #aab8cc;
            margin-bottom: 45px;
        }

        /* TECHNOLOGY CARDS */
        .card-container {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 30px;
        }

        .card {
            background: #121e35;
            border-radius: 15px;
            overflow: hidden;
            border: 1px solid #233652;
            transition: 0.4s;
        }

        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 30px #00d9ff33;
            border-color: #00d9ff;
        }

        .card img {
            width: 100%;
            height: 220px;
            object-fit: cover;
        }

        .card-content {
            padding: 25px;
        }

        .card-content h3 {
            color: #00d9ff;
            font-size: 22px;
            margin-bottom: 12px;
        }

        .card-content p {
            color: #c0ccdd;
            margin-bottom: 15px;
        }

        .card-content a {
            color: #00d9ff;
            text-decoration: none;
            font-weight: bold;
        }

        /* ABOUT SECTION */
        .about {
            text-align: center;
            padding: 80px 15%;
            background: #101a30;
        }

        .about p {
            color: #c0ccdd;
            max-width: 750px;
            margin: 25px auto 30px;
            font-size: 17px;
        }

        /* FOOTER */
        footer {
            background: #050914;
            text-align: center;
            padding: 30px 15px;
            color: #aab8cc;
        }

        footer h3 {
            color: white;
            margin-bottom: 10px;
        }

        footer span {
            color: #00d9ff;
        }

        footer p {
            margin: 5px;
            font-size: 14px;
        }

        /* RESPONSIVE DESIGN */
        @media (max-width: 900px) {
            .card-container {
                grid-template-columns: repeat(2, 1fr);
            }

            .hero h1 {
                font-size: 48px;
            }
        }

        @media (max-width: 600px) {
            nav {
                flex-direction: column;
                gap: 15px;
            }

            .nav-links {
                gap: 12px;
                flex-wrap: wrap;
                justify-content: center;
            }

            .hero {
                min-height: 75vh;
                text-align: center;
                justify-content: center;
            }

            .hero h1 {
                font-size: 38px;
            }

            .hero p {
                font-size: 15px;
            }

            .card-container {
                grid-template-columns: 1fr;
            }

            .section-title {
                font-size: 28px;
            }

            .about {
                padding: 60px 8%;
            }
        }

    </style>
</head>

<body>

    <!-- NAVIGATION -->
    <header>
        <nav>
            <h2 class="logo">TECH<span>SHOWCASE</span></h2>

            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#technology">Technologies</a></li>
                <li><a href="#gadgets">Gadgets</a></li>
                <li><a href="#about">About</a></li>
            </ul>
        </nav>
    </header>

    <!-- HOME SECTION -->
    <section class="hero" id="home">
        <div class="hero-content">

            <h1>EXPLORE THE <span>FUTURE</span></h1>

            <p>
                Discover modern technologies, innovative gadgets,
                and amazing inventions that are changing our world.
                Experience the future of technology today!
            </p>

            <a href="#technology" class="btn">Explore Now</a>

        </div>
    </section>

    <!-- TECHNOLOGY SECTION -->
    <section class="section" id="technology">

        <h2 class="section-title">Modern Technologies</h2>

        <p class="subtitle">
            Discover the technologies shaping our future.
        </p>

        <div class="card-container">

            <div class="card">
                <img src="https://images.unsplash.com/photo-1677442136019-21780ecad995?w=600"
                     alt="Artificial Intelligence">

                <div class="card-content">
                    <h3>Artificial Intelligence</h3>

                    <p>
                        AI allows machines to learn, think, and
                        perform tasks that normally require
                        human intelligence.
                    </p>

                    <a href="#about">Learn More →</a>
                </div>
            </div>

            <div class="card">
                <img src="https://images.unsplash.com/photo-1485827404703-89b55fcc595e?w=600"
                     alt="Robotics">

                <div class="card-content">
                    <h3>Robotics</h3>

                    <p>
                        Robots help people complete difficult tasks
                        in industries, healthcare, and everyday life.
                    </p>

                    <a href="#about">Learn More →</a>
                </div>
            </div>

            <div class="card">
                <img src="https://images.unsplash.com/photo-1518770660439-4636190af475?w=600"
                     alt="Computer Technology">

                <div class="card-content">
                    <h3>Computer Technology</h3>

                    <p>
                        Modern computers provide powerful performance
                        for work, communication, and entertainment.
                    </p>

                    <a href="#about">Learn More →</a>
                </div>
            </div>

        </div>
    </section>

    <!-- GADGETS SECTION -->
    <section class="section" id="gadgets">

        <h2 class="section-title">Latest Gadgets</h2>

        <p class="subtitle">
            Smart devices designed to make life easier.
        </p>

        <div class="card-container">

            <div class="card">
                <img src="https://images.unsplash.com/photo-1511707171634-5f897ff02aa9?w=600"
                     alt="Smartphone">

                <div class="card-content">
                    <h3>Smartphones</h3>

                    <p>
                        Powerful mobile devices for communication,
                        photography, gaming, and productivity.
                    </p>
                </div>
            </div>

            <div class="card">
                <img src="https://images.unsplash.com/photo-1523275335684-37898b6baf30?w=600"
                     alt="Smartwatch">

                <div class="card-content">
                    <h3>Smartwatches</h3>

                    <p>
                        Wearable technology that tracks fitness,
                        health, notifications, and daily activities.
                    </p>
                </div>
            </div>

            <div class="card">
                <img src="https://images.unsplash.com/photo-1496181133206-80ce9b88a853?w=600"
                     alt="Laptop">

                <div class="card-content">
                    <h3>Laptops</h3>

                    <p>
                        Portable computers for students,
                        professionals, creators, and gamers.
                    </p>
                </div>
            </div>

        </div>
    </section>

    <!-- ABOUT SECTION -->
    <section class="about" id="about">

        <h2 class="section-title">Innovation for Tomorrow</h2>

        <p>
            Technology continues to transform the way we live,
            learn, work, and communicate. From artificial intelligence
            to smart gadgets, innovations create new opportunities
            and help build a better future for everyone.
        </p>

        <a href="#home" class="btn">Back to Top</a>

    </section>

    <!-- FOOTER -->
    <footer>

        <h3>TECH<span>SHOWCASE</span></h3>

        <p>Exploring Technology. Discovering Innovation.</p>

        <p>© 2026 Technology Showcase. All Rights Reserved.</p>

    </footer>

</body>
</html>
