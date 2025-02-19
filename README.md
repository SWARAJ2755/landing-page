<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elegant Themes Inspired Webpage</title>
    <style>
        /* Global Styles */
        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
            overflow-x: hidden;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        /* Header Styles */
        header {
            background: rgba(44, 43, 43, 0.5);
            padding: 1rem;
            text-align: center;
            position: sticky;
            top: 0;
            z-index: 1000;
            transition: background 0.3s ease;
        }

        header.scrolled {
            background: rgba(100, 98, 98, 0.9);
        }

        nav ul {
            list-style: none;
            padding: 0;
            display: flex;
            justify-content: center;
            margin: 0;
        }

        nav ul li {
            margin: 0 15px;
            transition: transform 0.3s ease;
        }

        nav ul li a {
            color: black;
            text-decoration: none;
            padding: 10px 15px;
            display: block;
            transition: color 0.3s ease, transform 0.3s ease, background 0.3s ease;
            opacity: 0.7;
        }

        nav ul li a:hover {
            color: #f54c8f;
            background-color: rgba(245, 76, 143, 0.1);
            transform: scale(1.05);
            opacity: 1;
        }

        nav ul li a.active {
            background-color: #f54c8f;
            color: white;
            opacity: 1;
        }

        /* Hero Section */
        .hero {
            background: url('https://images.pexels.com/photos/574071/pexels-photo-574071.jpeg?auto=compress&cs=tinysrgb&w=600') center/cover no-repeat fixed;
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5);
            z-index: 1;
        }

        .hero-content {
            position: relative;
            z-index: 2;
            opacity: 0;
            transform: translateY(20px);
            animation: slideUp 1s 0.5s forwards;
        }

        
       

        /* About Section */
        .slide-container {
            width: 100%;
            min-height: 100vh;
            display: flex;
            align-items: center;
            padding: 50px 0;
            background: #f5f5f5;
        }

        .about-section {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }

        .about-image {
            position: relative;
            width: 100%;
            aspect-ratio: 1;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }

        .about-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .about-content {
            padding: 20px;
        }

        .about-title {
            font-size: 2.5rem;
            margin-bottom: 20px;
            position: relative;
        }

        .about-title span {
            color: #f54c8f;
        }

        .about-description {
            color: #666;
            margin-bottom: 30px;
            font-size: 1.1rem;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            margin-bottom: 30px;
        }

        .skill-item {
            display: flex;
            align-items: center;
            font-weight: 500;
        }

        .skill-item::before {
            content: "»";
            margin-right: 10px;
            color: #f54c8f;
        }

        .download-cv {
            display: inline-block;
            padding: 12px 30px;
            background: #f54c8f;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            font-weight: 500;
            transition: transform 0.3s ease, background 0.3s ease;
        }

        .download-cv:hover {
            transform: translateY(-2px);
            background: #e0437f;
        }
        .h1{
            color: #f4f4f4;
            font-size: large;
        }
        
    </style>
</head>
<body>
    <header id="header">
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="backpage.html">About</a></li>
                <li><a href="resume.html">Resume</a></li>
                <li><a href="my work.html">Services</a></li>
                <li><a href="">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero" id="home">
        <div class="hero-content">
            
        </div>
        <h1><strong>I AM DEVLOPER.......</strong></h1>
    </section>

    <section id="about" class="slide-container">
        <div class="about-section">
            <div class="about-image">
                <img src="https://st5.depositphotos.com/20923550/70483/v/450/depositphotos_704830854-stock-illustration-hipster-man-face-icon-vector.jpg" alt="Developer Profile">
            </div>
            <div class="about-content">
                <h2 class="about-title">ABOUT <span>ME</span></h2>
                <p class="about-description">
                    Hello! I'm a web developer, passionate about crafting engaging digital experiences.
                </p>
                <div class="skills-grid">
                    <div class="skill-item">Web Development</div>
                    <div class="skill-item">SEO</div>
                    <div class="skill-item">Social Media Marketing</div>
                    <div class="skill-item">Content Generation</div>
                </div>
                <a href="#" class="download-cv">Download CV</a>
            </div>
        </div>
    </section>
</body>
</html>
